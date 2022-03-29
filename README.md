[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

# Awesome errors

## Docker

### `standard_init_linux.go:228: exec user process caused: exec format error`

#### 1) The image was build for a different plattform

E.g. you have build the plattform on MacOS with M1 chip and need to rebuild it with the correct architecture.

```
# Add the --plattform  
docker buildx build --platform=linux/amd64 -t image-name:version .
```

* https://stackoverflow.com/a/70614305

