# 🦀 Week 2: Variables, Constants, Functions, Clippy & Modules

This week I worked through **Exercise A: Variables** from the [Ultimate Rust Crash Course](https://www.udemy.com/course/ultimate-rust-crash-course/).

---

## ✅ Exercise: Variables and Constants

```rust
const STARTING_MISSILES: i32 = 8;
const READY_AMOUNT: i32 = 2;

fn main() {
    let (mut missiles, ready): (i32, i32) = (STARTING_MISSILES, READY_AMOUNT);
    
    println!("Firing {} of my {} missiles...", ready, missiles);
    
    missiles -= ready;
    
    println!("{} missiles left", missiles);
}
```

---

## 🧠 Key Concepts Practiced

- **Constants**: Immutable and must have type annotations
- **Mutability**: Use `mut` to make variables changeable
- **Pattern Matching for Binding**: Clean variable unpacking
- **Formatted Output**: `println!` with `{}` placeholders

---

## 🔧 Functions

Created reusable functions to compute area and volume:

```rust
fn area_of(x: i32, y: i32) -> i32 {
    x * y
}

fn volume(x: i32, y: i32, z: i32) -> i32 {
    x * y * z
}
```

---

## 🧼 Using `cargo clippy`

Clippy helped improve code style:

- Remove `return` on last lines
- Use `_` for ignored variables
- Inline one-time bindings
- Prefer `format!` over string concatenation

Run it with:

```sh
cargo clippy
```


---

## 📘 What’s Next

Next week: **Scalar and Compound Types**  
→ Integers, floats, booleans, characters, tuples, arrays
