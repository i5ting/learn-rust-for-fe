## clap

https://docs.rs/clap/latest/clap/

## 小技巧

cargo-debug 里 ctrlc 做法

```rust
// Override ctrl+c handler to avoid premature exit
// TODO: this... doesn't stop the rust process exiting..?
ctrlc::set_handler(move || {
    warn!("CTRL+C");
    let mut then = b.lock().unwrap();
    let now = SystemTime::now();
    if now.duration_since(*then).unwrap() > Duration::from_secs(1) {
        std::process::exit(0);
    } else {
        *then = now;
    }
}).expect("Error setting Ctrl-C handler");
```

## 简单的命令

https://github.com/JoshMcguigan/cargo-run-script/blob/master/src/main.rs

## 序列化

https://github.com/serde-rs/serde
