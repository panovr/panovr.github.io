---
layout: post
title: Install Go Tools on VSCode
date:   2020-03-13 11:06:00
categories: Go
---

## Install Go Tools on VSCode

```
Enter %GOPATH%\src\，and create golang.org\x directory
cd %GOPATH%\src\golang.org\x
git clone https://github.com/golang/tools.git
git clone https://github.com/golang/mod.git
git clone https://github.com/golang/xerrors
```

If all goes well, you should see the output:
```
go.toolsGopath setting is not set. Using GOPATH /home/ylzhao/go
Installing 7 tools at /home/ylzhao/go/bin in module mode.
  gocode
  gopkgs
  go-outline
  gocode-gomod
  godef
  goimports
  golint

Installing github.com/mdempsky/gocode SUCCEEDED
Installing github.com/uudashr/gopkgs/v2/cmd/gopkgs SUCCEEDED
Installing github.com/ramya-rao-a/go-outline SUCCEEDED
Installing github.com/stamblerre/gocode SUCCEEDED
Installing github.com/rogpeppe/godef SUCCEEDED
Installing golang.org/x/tools/cmd/goimports SUCCEEDED
Installing golang.org/x/lint/golint SUCCEEDED

All tools successfully installed. You are ready to Go :).
```

Otherwise, for example, if go-diff install failed, first try:
```
go get -u github.com/sergi/go-diff/...

```

If that failed, then try:
```
Enter %GOPATH%\src\, and create github.com\sergi\ directory
cd %GOPATH%\src\github.com\sergi
git clone https://github.com/sergi/go-diff.git
go install github.com/sergi/go-diff
```

For others you can try:
```
Enter %GOPATH%\src\, and create github.com\sqs\ directory
cd %GOPATH%\src\github.com\sqs
git clone https://github.com/sqs/goreturns.git
go install github.com/sqs/goreturns
Enter %GOPATH%\src\, and create github.com\ramya-rao-a directory
cd %GOPATH%\src\github.com\ramya-rao-a
git clone https://github.com/ramya-rao-a/go-outline.git
go install github.com/ramya-rao-a/go-outline
```
