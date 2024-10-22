### Rust を WebAssembly で動かす

1. git clone

   ```bash
   git clone git@github.com:ys39/rust-wasm-practice.git
   cd rust-wasm-practice
   ```

2. http サーバの起動

   ```bash
   docker run --rm -p 8000:8000 \
   -v "$(pwd)":/usr/src/app \
   -w /usr/src/app python:3 python -m http.server 8000
   ```

3. `http://localhost:8000`にアクセスして確認
