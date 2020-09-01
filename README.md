# Gomobile Bug


This project has a very simple Go package that is called from Swift code. The package only has one function.

The error occurs when running on real hardware (iPhone X, iOS 13.6) but not the simulator. macOS: 10.15.6

On startup, the following appears in the debug output:

`runtime/cgo: chdir(/private/var/containers/Bundle/Application/3CB0E6B1-721E-45F6-9C38-CA0EB8D971E6/GoMobile%20Bug.app) failed`

This is my `go env`:

```
GO111MODULE="on"
GOARCH="amd64"
GOBIN=""
GOCACHE="/Users/<username>/Library/Caches/go-build"
GOENV="/Users/<username>/Library/Application Support/go/env"
GOEXE=""
GOFLAGS=""
GOHOSTARCH="amd64"
GOHOSTOS="darwin"
GOINSECURE=""
GOMODCACHE="/Users/<username>/dev/gowksp/pkg/mod"
GONOPROXY=""
GONOSUMDB=""
GOOS="darwin"
GOPATH="/Users/<username>/dev/gowksp"
GOPRIVATE=""
GOPROXY="https://proxy.golang.org,direct"
GOROOT="/usr/local/go"
GOSUMDB="sum.golang.org"
GOTMPDIR=""
GOTOOLDIR="/usr/local/go/pkg/tool/darwin_amd64"
GCCGO="gccgo"
AR="ar"
CC="clang"
CXX="clang++"
CGO_ENABLED="1"
GOMOD="/Users/<username>/dev/gowksp/src/github.com/curyous/adder/go.mod"
CGO_CFLAGS="-g -O2"
CGO_CPPFLAGS=""
CGO_CXXFLAGS="-g -O2"
CGO_FFLAGS="-g -O2"
CGO_LDFLAGS="-g -O2"
PKG_CONFIG="pkg-config"
GOGCCFLAGS="-fPIC -m64 -pthread -fno-caret-diagnostics -Qunused-arguments -fmessage-length=0 -fdebug-prefix-map=/var/folders/z8/x3j7np6x1cjbm_44396n2f680000gn/T/go-build960861663=/tmp/go-build -gno-record-gcc-switches -fno-common"
```