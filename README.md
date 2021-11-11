<p align=center><a href="https://learn.srlinux.dev"><img src=https://gitlab.com/rdodin/pics/-/wikis/uploads/00f61ff15f4f165c89174c46a5201820/srl-ndk-proto.svg?sanitize=true/></a></p>

[![Docs](https://img.shields.io/badge/Docs-learn.srlinux.dev-blue?style=flat-square&color=00c9ff&labelColor=bec8d2)](https://learn.srlinux.dev/ndk/intro/)

---

The Nokia SR Linux [NetOps Development Kit (NDK)](https://learn.srlinux.dev/ndk/intro/) allows operators to program high-performance, integrated agents that run alongside the Nokia Service Router Linux (SR Linux). This repository provides `.proto` files that define the gRPC APIs used with the NDK.
 
NDK protobufs are common across all SR Linux hardware platforms.

## Repository structure
The main branch of this repository contains only the documentation. To reveal the proto files for a given release select the tag that matches the SR Linux release version.

The tags match the SR Linux release version, for instance the tag `v21.6.2` corresponds to the SR Linux release 21.6.2.

## Code generation
Protocol buffers support generated code in many languages - Java, Python, Objective-C, C++, Dart, Go, Ruby, C# with more language to come.

Since NDK is defined with protocol buffers, SR Linux application developers can pick and choose any supported language when developing their apps.

Currently Nokia SR Linux team maintains the following generated language bindings for NDK:

- [srlinux-ndk-go](https://github.com/nokia/srlinux-ndk-go) - Go bindings
- [srlinux-ndk-py](https://github.com/nokia/srlinux-ndk-py) - Python bindings

To generate NDK code in other languages, consult with the official [protocol buffers documentation](https://developers.google.com/protocol-buffers/docs/tutorials) for a given language.

## Download
There are several ways to download the proto files for a specific SR Linux release. The below examples are provided for `v21.6.2` version.

### Clone with git
If git is installed it is possible to clone the protos for a specific release with the following command:
```
git clone -b v21.6.2 --depth 1 https://github.com/nokia/srlinux-ndk-protobufs
```

### Download archives
To download the proto files for a specific release in the `zip` or `tgz` containers navigate to the github [`tags`](https://github.com/nokia/srlinux-ndk-protobufs/tags) page which contains the links to the archives.

If needed, the download link can be programmatically derived using the following rule:

**for zip**
`https://github.com/nokia/srlinux-ndk-protobufs/archive/tags/` + `$tag` + `.zip`

**for tar.gz**
`https://github.com/nokia/srlinux-ndk-protobufs/archive/tags/` + `$tag` + `.tar.gz`
