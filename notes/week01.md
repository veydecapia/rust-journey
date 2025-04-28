# Rust Journey – Week 1: Installing, Cloning, and First Impressions

A documentation of my first week transitioning from QA to Rust development, following [The Ultimate Rust Crash Course](https://www.udemy.com/course/ultimate-rust-crash-course/) and *The Rust Programming Language Book*.

---

## ✅ What I Did

- Cloned the official crash course repo  
  👉 https://github.com/CleanCut/ultimate_rust_crash_course  
- Installed Rust using `rustup`
- Configured VS Code with Rust Analyzer + CodeLLDB
- Ran the multilingual “hello” example
- Explored key concepts like variables, constants, scope, and memory safety

---

## ⚙️ Tools Used

- **OS:** macOS  
- **Editor:** VS Code  
- **Extensions:** Rust Analyzer, CodeLLDB  
- **Commands:** `rustup`, `cargo`, `rustc`

---

## 🧠 Key Concepts

### Cargo

- Ran `cargo build`, `cargo run`, `cargo check`
- Learned the importance of the `Cargo.toml` manifest file

---

### Variables

- Immutable by default
- Use `mut` to allow reassignment

```rust
let mut score = 0;
score += 1;
```

---

### Constants

- Declared using `const`, requires type
- All uppercase with underscores
- Inlined at compile time

```rust
const WARP_FACTOR: f64 = 9.9;
```

---

### Scope

- Block-based variable lifetime
- No garbage collector — values are dropped at the end of the block

```rust
{
    let message = "hello";
}
// message is now out of scope
```

---

### Shadowing

- You can redeclare a variable with the same name

```rust
let spaces = "   ";
let spaces = spaces.len();
```

---

### Memory Safety

- Ownership and borrowing enforced at compile time
- Prevents double-free, dangling pointers, and use-after-free errors

```rust
let s1 = String::from("hello");
let s2 = s1;
// println!("{}", s1); // ❌ invalid, s1 was moved
```

---

## 🧩 First Gotcha

Ran `cargo run` in the wrong folder:

```bash
cd examples
cargo run
```

Error:

```
error: could not find `Cargo.toml`
```

**Fix:**

```bash
cd examples/hello
cargo run
```

---

## 📚 References

- Week 1 Notes: [notes/week01.md](notes/week01.md)  
- Medium article: [Rust Journey – Week 1](https://medium.com/@harveydecapia/rust-journey-week-1-installing-cloning-and-first-impressions-4c6749fe10f8)

---

## 📬 Follow the Journey

- [LinkedIn](https://linkedin.com/in/harveydecapia)  
- [GitHub](https://github.com/veydecapia)

> “QA taught me how to think about software. Rust is teaching me how to build it.”
