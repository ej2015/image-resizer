# A simple image resizer server

## Description
It uses govips (a wrapper of libvips). It is based on [this blog](https://karthikkaranth.me/blog/image-resizing-server-go-libvips/)

## Compilation
CGO_CFLAGS_ALLOW=-Xpreprocessor go build main.go

## Usage
Pass in the image url in query params. e.g. 

```
http://localhost:4444/?width=194&height=149&url=https://upload.wikimedia.org/wikipedia/commons/e/ee/Grumpy_Cat_by_Gage_Skidmore.jpg
```
