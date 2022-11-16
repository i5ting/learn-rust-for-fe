# 入门

## rustc

## rustdoc

- https://doc.rust-lang.org/std/
- https://docs.rs/

## cargo

## 断点调试

### jetbrains rust 插件

https://plugins.jetbrains.com/plugin/8182-rust/docs/rust-debugging.html

### vscode

在 VS Code 里， Ctrl-P (在 macOS 下 Command P )，执行下面的命令

> ext install rust-lang.rust

### rust-debug

https://dev.to/rogertorres/debugging-rust-with-vs-code-11dj

### cargo-debug + vscode attach

https://github.com/cargo-bins/cargo-debug

```
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "lldb",
            "request": "launch",
            "name": "Debug executable 'hello-world'",
            "cargo": {
                "args": [
                    "build",
                    "--bin=hello-world",
                    "--package=hello-world"
                ],
                "filter": {
                    "name": "hello-world",
                    "kind": "bin"
                }
            },
            "args": [],
            "cwd": "${workspaceFolder}"
        },
        {
            "type": "lldb",
            "request": "launch",
            "name": "Debug unit tests in executable 'hello-world'",
            "cargo": {
                "args": [
                    "test",
                    "--no-run",
                    "--bin=hello-world",
                    "--package=hello-world"
                ],
                "filter": {
                    "name": "hello-world",
                    "kind": "bin"
                }
            },
            "args": [],
            "cwd": "${workspaceFolder}"
        }
    ]
}
```

启动`cargo debug`，然后在 vscode 里 attach 到具体进程即可。

## 测试代码

## 性能压测

## 添加一个文件

主要是引出模块
