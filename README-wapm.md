# coreutils

Core utils for WebAssembly and WASI

```bash
wapm install coreutils
```

**Original Source**: https://github.com/uutils/coreutils

**Modifications**: We made some changes to adapt the codebase to the [WASI interface](https://wapm.io/interface/wasi).

## Running

The following commands are available:

```bash
ls
cat
echo
mv
env
mkdir
basename
dirname
base32
base64
sum
printf
wc
pwd
```

## Building

The following script will build the binary:

```bash
cargo build --features "ls cat echo mv env mkdir basename dirname base64 base32 sum printf wc pwd" --no-default-features --target wasm32-wasi --release
```
