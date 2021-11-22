说rust是webassembly未来，目前看还不是，多语言里大家几率不会差太多。web server已经卷死了，无机会。云原生是go的地盘，难下手，机器学习py才是王者，大数据和后端Java天下，可玩的有限。综上，JS依然是应用软件最好的选择。但rust做基建，提供更好的开发体验，倒是大有可为的。

当然rust是写前端基建，是裆下趋势。 

Rust语言在前端工具链的影响越来越大，目前可以看到next.js对rust重仓，招揽大量人才，swc作者，rollup作者等等，未来可能是一个很好的解决前端体验的方向

《Rust Is The Future of JavaScript Infrastructure》  https://leerob.io/blog/rust  ，作者是Vercel的开发者关系主管，这篇文章和叔的观点一样，自备梯子。

很多东西都是上错花轿嫁对郎，比如mvc，比node，如今又多了rust。必然雄起！未来随着webassembly普及，rust才能变成应用级别的。

## 前端工具链项目

- https://github.com/volta-cli/volta 对标nvm+npm
    - https://github.com/Schniz/fnm
- https://github.com/justjavac/postcss-rs  对标postcss
- https://github.com/CGQAQ/rusty-source-map 对标[Mozilla/source-map](https://github.com/mozilla/source-map)
- https://github.com/swc-project/swc  对标ts/babel
    - swcpack： SWC的bundle工具，类似于webpack
    - swc-css: SWC的CSS parser，类似PostCSS
    - Deno: JS/TS的runtime，但是也提供诸如linter, code formatter, docs generator, bundle这些功能， 当然基于SWC
    - Rome： Babel的作者Sebastian创建，目前已经在进行Rust重写，基于rslint_parser(https://github.com/rslint/rslint)，项目代码 https://github.com/rome/tools
    - dprint： 基于SWC构建，提供类似Prettier的功能，但是比 Prettier 快30倍
    - Parcel 2: 基于SWC，打包性能提升10倍
    - https://github.com/Brooooooklyn/swc-node
    - https://github.com/TypeStrong/ts-node 支持swc
- https://github.com/g-plane/browserslist-rs 对标 [browserslist](https://github.com/browserslist/browserslist)
- https://github.com/HerringtonDarkholme/vue-compiler 对标 vue-template-compiler
- https://github.com/rslint/rslint 对标eslint
- https://github.com/yisibl/resvg-js  A high-performance SVG renderer, powered by Rust based resvg and napi-rs.
- https://napi.rs/ NAPI-RS: a minimal library for building pre-compiled Node.js addons in Rust 
- https://neon-bindings.com/ Neon: Electrify your Node with the power of Rust 
- https://github.com/tauri-apps/tauri Tauri: Electron alternative Tauri written in Rust
- https://github.com/boa-dev/boa  Boa (JS engine in Rust)
- https://github.com/DrSensor/rs-jest 一个用于跑 Rust 单元测试的 jest transformer，安装之后只需要简单配置一下 jest.config.js 即可。很老，可能需要更新
- https://github.com/image-rs/image-png PNG decoding and encoding library in pure Rust
- https://github.com/gfx-rs/wgpu Safe and portable GPU abstraction in Rust, implementing WebGPU API.
- https://github.com/rust-analyzer/rust-analyzer A Rust compiler front-end for IDEs

## 开发者

- https://github.com/justjavac
- https://github.com/yisibl
- https://github.com/Brooooooklyn

## 工具

- https://searchfox.org/

## 参考

- https://nextjs.org/blog/next-12#faster-builds-and-fast-refresh-with-rust-compiler
  - 我看Next.js：一个更现代的海王 https://mp.weixin.qq.com/s/5Ir7EoHLo37bs6W5WNa-Tw

其他大家补充，欢迎pr
