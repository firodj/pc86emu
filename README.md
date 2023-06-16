# pc86emu

## Unicorn-Engine

To use unicorn engine, build `libunicorn.dll` first.

Go to `cd $USERPROFILE/go/pkg/mod/github.com/unicorn-engine/unicorn@your_version`.

Read `docs/COMPILE.md`, for Windows UCRT64/MSYS, after downloading toolchains:

```sh
$ mkdir build
$ cmake -G Ninja ..
$ ninja -C .
```

Make sure `libunicorn.dll` created and copy to root unicorn for building.
Please see where `LDFLAGS -L` expect to find on file `bindings/go/unicorn/unicorn.go`.
Also copy to root of this project for running.

## Building

```sh
$ go build cmd/hello/main.go -o hello.exe
$ ./hello.exe
```

