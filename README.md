# 重要提醒 ProxySwitchy 仓库说明

本仓库的默认分支仅用于提醒，**不包含任何代码**。

### 获取代码
- 活跃维护分支：**[zero-peak](../../tree/zero-peak)** （同步自 zero-peak/ZeroOmega）
- 停更原版分支：**[FelisCatus](../../tree/FelisCatus)** （同步自 FelisCatus/SwitchyOmega）

### ⚠️ 禁止在网页上使用 Sync fork 按钮
本仓库的代码分支并非父仓库的直接衍生版，使用网页同步会破坏分支历史。
更新请使用命令行：
```bash
# 同步 zero-peak
git checkout zero-peak
git -c http.proxy=http://127.0.0.1:10808 -c https.proxy=http://127.0.0.1:10808 pull zero-peak master
git -c http.proxy=http://127.0.0.1:10808 -c https.proxy=http://127.0.0.1:10808 push origin zero-peak
```

## ⚠️ 【最高优先级警告】严禁操作
1. **禁止在 zero-peak / FelisCatus 任意分支点击网页 Sync fork**
该功能仅绑定原始上游 FelisCatus/SwitchyOmega，一旦执行会覆盖 zero-peak 第三方定制代码，引发大规模代码丢失与冲突。
2. 所有上游代码更新，仅允许通过本地 Git 命令行同步，禁止网页一键同步 Fork。

## 分支介绍
1. 【主力维护】`zero-peak`
同步上游仓库：zero-peak/ZeroOmega  master
持续迭代更新，为当前可用最新版本。
2. 【存档归档】`FelisCatus`
原版 SwitchyOmega 官方源码，项目已停止更新，仅用于源码备份、历史查阅，不再维护。
3. 【本分支 main】
仅为仓库导航+风险警示页，不包含任何项目源代码，请勿在此分支开发、合并代码。

## 如何获取源码
1. Git 克隆仓库后，手动执行切换分支命令：
`git checkout zero-peak`
2. 网页端直接点击分支下拉，切换至 `zero-peak` 查看、下载最新源码。
