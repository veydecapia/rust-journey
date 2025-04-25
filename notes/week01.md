# 🦀 Rust Learning & Setup Journey

## 📅 Week 1 - Day 1

## ✅ Initial Setup

### Cloned Course Repository
```bash
git clone https://github.com/CleanCut/ultimate_rust_crash_course.git
cd ultimate_rust_crash_course
```

### Installed Rust using rustup
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

### Added Rust to PATH via `.zshrc`
```bash
nano ~/.zshrc
# Added:
export PATH="$HOME/.cargo/bin:$PATH"
source ~/.zshrc
```

### Verified installation
```bash
rustc --version
cargo --version
```

## 📁 Navigating Project Structure

### 🧠 Context:
After setting up Rust and cloning the course repo, I was eager to run my first Rust project. I navigated into the `examples` folder, expecting things to just work with a simple `cargo run`.

However, Rust projects rely on a `Cargo.toml` file, which acts as the project manifest — defining dependencies, project metadata, and configuration. Without this file in the current or parent directory, Cargo can’t function properly.

This led to my first "gotcha" moment.

### Error encountered:
```
error: could not find `Cargo.toml` in `/Users/harveydecapia/Documents/GitHub/ultimate_rust_crash_course/examples` or any parent directory
```

### Reason:
Ran `cargo run` in a folder **without** `Cargo.toml`

### Fix:
Changed directory to correct path with `Cargo.toml`
```bash
cd /Users/harveydecapia/Documents/GitHub/ultimate_rust_crash_course/examples/hello
cargo run
```

## 📦 Project Details

`Cargo.toml` contents:
```toml
[package]
name = "hello"
version = "0.1.0"
edition = "2021"

[dependencies]
rand = "0.8"
```

## Screenshot: First Successful Run

![First Cargo Run Output](https://github.com/user-attachments/assets/b2010844-4ed9-48b8-aa3f-dda758c037d1)
## 🏁 Next Steps
- Continue working on `hello` example
- Try modifying `main.rs` and running `cargo run`
- Document progress here regularly

