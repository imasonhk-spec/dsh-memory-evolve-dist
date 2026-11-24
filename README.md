# dsh-memory-evolve（发布产物仓库）

本仓库**只存放发布产物**，源码与开发历史在私有仓库 `imasonhk-spec/dsh-memory-evolve`。

| 项 | 值 |
|---|---|
| 包名 | `dsh-memory-evolve` |
| 版本 | `0.3.0` |
| 许可证 | MIT（见 [LICENSE](./LICENSE)） |
| 产物 | [`dsh-memory-evolve-0.3.0.tgz`](./dsh-memory-evolve-0.3.0.tgz) |

## 为什么有这个仓库

`dsh-memory-evolve` 原仓库为私有，`pnpm` 从 `github:` 协议安装会走 `git+ssh`，在没有 SSH 凭据的机器上直接失败。为了让它能被**公开、自动安装**（例如作为 `@local/dsh-ms-dev-preset` 的依赖），这里只公开打包产物 tarball。

## 安装

```bash
pnpm add https://github.com/imasonhk-spec/dsh-memory-evolve-dist/raw/main/dsh-memory-evolve-0.3.0.tgz
# 或
npm i https://github.com/imasonhk-spec/dsh-memory-evolve-dist/raw/main/dsh-memory-evolve-0.3.0.tgz
```

## 说明

- 与私有仓库 0.3.0 相比，仅把 `package.json` 的 `private` 置为 `false`（否则部分包管理器拒绝安装）。
- 本仓库不包含 `.git` 历史、开发脚本与任何凭据；如发现内容问题请开 issue。
