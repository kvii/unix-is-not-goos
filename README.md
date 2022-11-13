# unix-is-not-goos

Some code showing that unix is not GOOS.

Reference:
* [go don't support *_unix.go](https://github.com/golang/go/issues/51572)
* [Build_constraints](https://pkg.go.dev/cmd/go#hdr-Build_constraints)

```shell
# in *nix platform
$ export GOOS=windows && go run .
# demo
./code_windows.go:3:5: value redeclared in this block
        ./code_unix.go:3:5: other declaration of value
```