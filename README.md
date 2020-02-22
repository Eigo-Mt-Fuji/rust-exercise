## README

* Let's start first [rust](https://doc.rust-lang.org/1.0.0/book/hello-cargo.html) fast.


## Install

```bash
curl https://sh.rustup.rs -sSf | sh
```

## Exercise
 
* Mkdir rust-exercise

```bash
mkdir -p rust-exercise
```

* Move into rust-exercise

```bash
cd ./rust-exercise
```

* Create file `Cargo.toml`

```bash
cat <<EOF > Cargo.toml
[package]

name = "efg-river"
version = "0.0.1"
authors = [ "Eigo Fujikawa <efg.river@gmail.com>" ]
EOF
```

* Mkdir src

```bash
mkdir -p src
```

* Create file ./src/main.rs with "Hello World" .

```bash
cat <<EOF > ./src/main.rs
fn main() {
    println!("Hello, world!");
}
EOF
```

* Build(debug)

```bash
cargo build
```

* Run(debug)

```bash
cargo run
```

* Run(debug) Output

```bash
EigonoMacBook-Pro:rust-exercise fujikawa$ cargo run
    Finished dev [unoptimized + debuginfo] target(s) in 0.05s
     Running `target/debug/efg-river`
Hello, world!
```


* Build(release)

```bash
cargo build --release
```

* Run(release)

```bash
cargo run --release
```

* Run(release) Output

```bash
EigonoMacBook-Pro:rust-exercise fujikawa$ cargo run --release
    Finished release [optimized] target(s) in 0.01s
     Running `target/release/efg-river`
Hello, world!
```
