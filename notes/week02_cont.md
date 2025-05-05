# 🦀 Rust Journey – Week 2 Continued  
## Primitive and Compound Types

This continuation of Week 2 explores how Rust handles core data types.  
If you haven’t read the first part yet, start here:  
👉 [Week 2: Variables, Constants, Functions, Cargo, Clippy](https://medium.com/@harveydecapia/rust-journey-week-2-variables-constants-functions-cargo-clippy-3bfe461c60cb)

---

### 📗 Medium Article

👉 [Rust Journey – Week 2 Continued: Primitive and Compound Types](https://medium.com/@harveydecapia/rust-journey-week-2-continued-primitive-and-compound-types-216f92502242)

---

### 🔹 Topics Covered

#### ✅ Primitive Types
- Signed and unsigned integers: `i32`, `u64`, etc.
- Default types: `i32` for integers, `f64` for floats
- Casting between types using `as`
- Floating-point numbers with leading zero (`0.1`, not `.1`)
- Readability with numeric underscores (`1_000_000`)
- Booleans: `true`, `false` (lowercase only)
- Characters (`char`): Unicode, 4 bytes, single quotes

#### ✅ Compound Types
- Tuples: fixed length, mixed types, accessed by index or destructuring
- Arrays: same type, fixed length, stack-allocated

#### ⚠️ Array Limitations
- Traits like `Debug`, `Clone`, and `PartialEq` are only auto-implemented for arrays up to 32 elements
- Larger arrays are supported via const generics (since Rust 1.51), but some libraries still impose limits
- Use `Vec<T>` or slices if you need more flexibility  
- Discussion thread: [Reddit – Why are Rust arrays limited to 32 values?](https://www.reddit.com/r/rust/comments/cwxeye/why_are_rust_arrays_limited_to_32_values/?rdt=39906)

---

### 🧠 Key Takeaway

> Rust forces you to be explicit with types.  
> That can feel strict at first, but it leads to safer, more predictable code.

---

### 🔜 Up Next

[Week 3 – Control Flow](../week03.md) (coming soon)

---

Back to main log:  
🔗 [Rust Journey: Weekly Progress Log (No Paywall)](https://medium.com/@harveydecapia/rust-journey-weekly-progress-log-no-paywall-31455af64c1c)
