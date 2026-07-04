# ⚠️ 重要提醒

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
