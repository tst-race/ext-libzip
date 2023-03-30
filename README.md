# libzip for RACE

This repo provides scripts to custom-build the
[libzip library](https://libzip.org/) for RACE.

## License

The libzip library is licensed under the 3-Clause BSD license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

libzip has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build libzip.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-libzip.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-libzip
```

## Platforms

libzip is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`
* `android-x86_64`
* `android-arm64-v8a`

## How It Is Used

libzip is used directly by the RACE core and slothy.
