## Basic 
###  Set-up project directory 
```bash
mkdir ~/pro_dir
cd ~/pro_dir
```

### Set-up Project
```
cargo new hello
```

then,
	open the `main.rs` in the `src` folder of the project.
		Something like this should be there 
```rust
fn main() {
    println!("Hello, world!");
}
```

### Build and Run the program
```bash
cargo build
cargo run
```

Or Compiling 
```shell
rustc main.rs
```
## 