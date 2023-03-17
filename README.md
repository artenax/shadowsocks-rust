Shadowsocks is a fast tunnel proxy that helps you bypass firewalls

## Usage
```
sslocal -b "127.0.0.1:1080" --server-url "ss://ID"
```
You can decode ss:// into config using [Base64 Decoder](http://4mhz.de/b64dec.html). Or echo CODE | base64 -d

## Cross-compilation
```
# Install mingw-i686 from the package manager
rustup target add i686-pc-windows-gnu
rustup target add i686-unknown-linux-musl
cargo build --release --target i686-pc-windows-gnu
cargo build --release --target i686-unknown-linux-musl
```
