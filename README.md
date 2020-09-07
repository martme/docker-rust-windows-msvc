# Docker Image for Compiling Rust Code on Windows

500 most popular crates prefetched from crates.io

## Build
```
docker build -t rust-windows-msvc:latest .
```

## Run

Mount source files, e.g. the directory containing Cargo.toml into `C:\Source`.

```powershell
docker run -v "$(Get-Location):C:\Source" rust-windows-msvc cargo build
```
