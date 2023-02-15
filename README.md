说 Rust 是 WebAssembly 未来，目前看还不是，多语言里大家几率不会差太多。Web Server 已经卷死了，无机会。云原生是 Go 的地盘，难下手，机器学习 Python 才是王者，大数据和后端 Java 天下，可玩的有限。综上，JavaScript 依然是应用软件最好的选择。但 Rust 做基建，提供更好的开发体验，倒是大有可为的。

当然 Rust 是写前端基建，是当下趋势。

Rust 语言在前端工具链的影响越来越大，目前可以看到 Next.js 对 Rust 重仓，招揽大量人才，swc 作者，rollup 作者等等，未来可能是一个很好的解决前端体验的方向。

《Rust Is The Future of JavaScript Infrastructure》（[原文](https://leerob.io/blog/rust) | [中文翻译](https://mp.weixin.qq.com/s?__biz=MzkxNDIzNTg4MA==&mid=2247485792&idx=1&sn=682a4dee7ce4d3b47a81baf9ebd7a98a) ) ，作者是 Vercel 的开发者关系主管，这篇文章和叔的观点一样，自备梯子。
很多东西都是上错花轿嫁对郎，比如 mvc，比如 Node，如今又多了 Rust。必然雄起！未来随着 WebAssembly 普及，Rust 才能变成应用级别的。

## 前端工具链项目

- https://github.com/volta-cli/volta 对标 nvm+npm
  - https://github.com/Schniz/fnm
- https://github.com/justjavac/postcss-rs 对标 postcss
- https://github.com/CGQAQ/rusty-source-map 对标 [Mozilla/source-map](https://github.com/mozilla/source-map)
- https://github.com/swc-project/swc 对标 ts/babel
  - swcpack： SWC 的 bundle 工具，类似于 Webpack
  - swc-css: SWC 的 CSS parser，类似 PostCSS
  - Deno: JS/TS 的 runtime，但是也提供诸如 linter, code formatter, docs generator, bundle 这些功能， 当然基于 SWC
  - Rome： Babel 的作者 Sebastian 创建，目前已经在进行 Rust 重写，基于 [rslint_parser](https://github.com/rslint/rslint)，项目代码 https://github.com/rome/tools
  - dprint： 基于 SWC 构建，提供类似 Prettier 的功能，但是比 Prettier 快 30 倍
  - Parcel 2: 基于 SWC，打包性能提升 10 倍
  - https://github.com/Brooooooklyn/swc-node
  - https://github.com/TypeStrong/ts-node 支持 swc
- https://github.com/g-plane/browserslist-rs 对标 [browserslist](https://github.com/browserslist/browserslist)
- https://github.com/HerringtonDarkholme/vue-compiler 对标 vue-template-compiler
- https://github.com/rslint/rslint 对标 eslint
- https://github.com/yisibl/resvg-js A high-performance SVG renderer, powered by Rust based resvg and napi-rs.
- https://napi.rs/ NAPI-RS: a minimal library for building pre-compiled Node.js addons in Rust
- https://neon-bindings.com/ Neon: Electrify your Node with the power of Rust
- https://github.com/tauri-apps/tauri Tauri: Electron alternative Tauri written in Rust
- https://github.com/boa-dev/boa Boa (JS engine in Rust)
- https://github.com/DrSensor/rs-jest 一个用于跑 Rust 单元测试的 jest transformer，安装之后只需要简单配置一下 jest.config.js 即可。很老，可能需要更新
- https://github.com/image-rs/image-png PNG decoding and encoding library in pure Rust
- https://github.com/gfx-rs/wgpu Safe and portable GPU abstraction in Rust, implementing WebGPU API.
- https://github.com/rust-analyzer/rust-analyzer A Rust compiler front-end for IDEs
- https://github.com/38/plotters Plotters is drawing library designed for rendering figures, plots, and charts, in pure rust. Plotters supports various types of back-ends, including bitmap, vector graph, piston window, GTK/Cairo and WebAssembly.
- https://github.com/leizongmin/htmlstream-rust Lightweight HTML parser
- https://github.com/djc/askama Type-safe, compiled Jinja-like templates for Rust
- https://github.com/facebook/relay/tree/v13.0.0-rc.1/compiler relay compiler was written in rust
- https://github.com/thedodd/trunk Build, bundle & ship your Rust WASM application to the web.
- https://github.com/yewstack/yew Rust / Wasm framework for building client web apps
- https://github.com/egoist/dum An npm scripts runner written in Rust.
- https://github.com/devongovett/tree-sitter-highlight A syntax highlighter for Node powered by Tree Sitter. Written in Rust.
- https://github.com/flo-l/jsonpp-rs UNIX style tool to pretty print json
- https://turbo.build/pack 对标 webpack 和 vite
- https://github.com/wooorm/mdxjs-rs markdown扩展

## 开发者

- https://github.com/justjavac
- https://github.com/yisibl
- https://github.com/Brooooooklyn

## 生态

- https://github.com/actix/actix Actor framework for Rust
- https://github.com/async-rs/async-std Async version of the Rust standard library
- https://github.com/rust-lang/cargo The Rust package manager
- https://github.com/crossbeam-rs/crossbeam Tools for concurrent programming in Rust
- https://github.com/denoland/rusty_v8 Rust bindings for the V8 JavaScript engine
- https://github.com/denoland/deno_lint Blazing fast linter for JavaScript and TypeScript written in Rust
- https://github.com/denoland/deno_bindgen Simplified glue code generation for Deno FFI libraries written in Rust.
- https://github.com/napi-rs/napi-rs A framework for building compiled Node.js add-ons in Rust via Node-API
- https://github.com/infinyon/node-bindgen Easy way to write Node.js module using Rust
- https://github.com/rayon-rs/rayon Rayon: A data parallelism library for Rust
- https://github.com/SergioBenitez/Rocket A web framework for Rust.
- https://github.com/Amanieu/parking_lot Compact and efficient synchronization primitives for Rust. Also provides an API for creating custom synchronization primitives.
- https://github.com/rustdesk/rustdesk Yet another remote desktop software
- https://github.com/rust-lang/rust-bindgen Automatically generates Rust FFI bindings to C (and some C++) libraries.
- https://github.com/serde-rs/serde Serialization framework for Rust
- https://github.com/tauri-apps/tauri Build smaller, faster, and more secure desktop applications with a web frontend.
- https://github.com/tokio-rs/tokio A runtime for writing reliable asynchronous applications with Rust. Provides I/O, networking, scheduling, timers, ...
- https://github.com/rustwasm/wasm-bindgen Facilitating high-level interactions between Wasm modules and JavaScript



## 工具

- https://searchfox.org/ Searchfox is a source code indexing tool for Mozilla Firefox. It indexes C++, Rust, and JavaScript code.
- https://github.com/meilisearch/MeiliSearch Powerful, fast, and an easy to use search engine
- https://github.com/editso/fuso 一款快速 🚀、稳定、跨平台、高效的内网穿透，端口转发工具
- https://github.com/clap-rs/clap A full featured, fast Command Line Argument Parser for Rust
- https://github.com/zellij-org/zellij A terminal workspace with batteries included
- https://github.com/nushell/nushell A new type of shell

## 参考

- https://kaisery.github.io/trpl-zh-cn/ Rust 官方教程中文翻译
- https://rustwiki.org/zh-CN/rust-by-example/ 通过例子学 Rust（官方教程翻译）
- https://rustcc.gitbooks.io/rustprimer/content/ 初学者教程（社区教程）
- https://github.com/wtklbm/rust-library-i18n/ Rust 标准库翻译
- https://course.rs/ Rust 语言圣经
- https://nextjs.org/blog/next-12#faster-builds-and-fast-refresh-with-rust-compiler
  - 我看 Next.js：一个更现代的海王 https://mp.weixin.qq.com/s/5Ir7EoHLo37bs6W5WNa-Tw
- https://vino.dev/blog/node-to-rust-day-1-rustup/ （自备梯子）
  - 24 天，从 Node 到 Rust
- https://www.youtube.com/playlist?list=PLai5B987bZ9CoVR-QEIN9foz4QCJ0H2Y8
  - 官方教程视频导读
- https://github.com/rust-unofficial/patterns A catalogue of Rust design patterns, anti-patterns and idioms
- https://www.youtube.com/playlist?list=PL3azK8C0kje1DUJbaOqce19j3R_-tIc4_ rust 编程语言入门教程，from Dave Young
- https://github.com/TheAlgorithms/Rust All Algorithms implemented in Rust
- https://github.com/rust-lang/rustlings Rust 小练习
- https://github.com/vinodotdev/node-to-rust From JavaScript to Rust ebook
- https://tourofrust.com Rust语言之旅, 在线从浅入深的练习常见语法
- https://github.com/sunface/rust-by-practice Rust 语言实战
- https://rusty.rs/about.html Rusty Book(锈书)

其他大家补充，欢迎 pr
