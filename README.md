Rust语言在前端工具链的影响越来越大，目前可以看到next.js对rust重仓，未来可能是一个很好的解决前端体验的方向

《Rust Is The Future of JavaScript Infrastructure》  https://leerob.io/blog/rust  ，作者是Vercel的开发者关系主管，这篇文章和叔的观点一样，自备梯子。

未来随着webassembly普及，rust才能变成应用级别的。

## 前端工具链项目

- https://github.com/volta-cli/volta 对标nvm+npm
    - https://github.com/Schniz/fnm
- https://github.com/justjavac/postcss-rs  对标postcss
- https://github.com/CGQAQ/rusty-source-map 对标[Mozilla/source-map](https://github.com/mozilla/source-map)
- https://github.com/swc-project/swc  对标ts/babel
    - swcpack： SWC的bundle工具，类似于webpack
    - swc-css: SWC的CSS parser，类似PostCSS
    - Deno: JS/TS的runtime，但是也提供诸如linter, code formatter, docs generator, bundle这些功能， 当然基于SWC
    - Rome： Babel的作者Sebastian创建，目前已经在进行Rust重写，应该会基于SWC，项目代码 https://github.com/rome/tools
    - dprint： 基于SWC构建，提供类似Prettier的功能，但是比 Prettier 快30倍
    - Parcel 2: 基于SWC，打包性能提升10倍
    - https://github.com/Brooooooklyn/swc-node
    - https://github.com/TypeStrong/ts-node 支持swc
- https://github.com/g-plane/browserslist-rs 对标 [browserslist](https://github.com/browserslist/browserslist)
- https://github.com/HerringtonDarkholme/vue-compiler 对标 vue-template-compiler
- https://github.com/rslint/rslint 对标eslint
- https://github.com/yisibl/resvg-js  A high-performance SVG renderer, powered by Rust based resvg and napi-rs.
- NAPI-RS: a minimal library for building pre-compiled Node.js addons in Rust https://napi.rs/
- Neon: Electrify your Node with the power of Rust https://neon-bindings.com/
- Tauri: Electron alternative Tauri written in Rust https://github.com/tauri-apps/tauri
- Boa (JS engine in Rust) – https://github.com/boa-dev/boa


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
