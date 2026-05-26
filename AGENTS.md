# AGENTS.md

## 子模组

本项目使用 Git 子模组管理关联仓库：

| 子模组 | 路径 | 用途 |
|--------|------|------|
| qtcloud-knowl | `apps/qtcloud-knowl` | 知识云平台应用 |
| knowl-toolkit | `packages/toolkit` | 知识工程工具包 SDK |
| gallery | `docs/gallery` | 知识工程工作案例展示 |
| examples-default | `examples/default` | 知识工程通用实验室 |
| context | `docs/context` | 知识工程语境文档 |

**子模组操作规范：**
- 拉取更新：`git submodule update --remote <path>`
- 修改子模组：进入子模组目录提交后，回到主仓库更新引用
- 初始化克隆：`git clone --recurse-submodules <repo-url>`

## 行为约束

- **禁止越界修改**：未经同意，不得修改本仓库之外的代码文件（包括 `qtcloud-devops` 工具、上级主仓库配置、其他子模组等）
- **发现问题**：可指出问题现象，但将修复决定权留给仓库负责人
