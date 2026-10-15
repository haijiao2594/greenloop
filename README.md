# 绿循 · 校园垃圾分类积分系统（GitHub Pages 版）

校园垃圾分类激励原型：活动方输入学号打卡发放积分（密码保护后台），学生通过分享链接查自己的积分与全校排名。

## 功能
- 活动方后台（密码保护）：打卡发分、手动调整、积分规则设置、记录导出 CSV、演示数据
- 学生公开页：查个人积分与排名、Top20 排行榜（学号脱敏）、`?sid=学号` 分享链接

## 部署（GitHub Pages）
1. 在 github.com 新建一个**公开**仓库（如 `greenloop`）
2. 把本目录内容推上去：
   ```
   git remote add origin https://github.com/<你的用户名>/greenloop.git
   git branch -M main
   git push -u origin main
   ```
3. 仓库 Settings → Pages → Source 选 `main` 分支 / `/(root)` → Save
4. 约 1 分钟后访问 `https://<你的用户名>.github.io/greenloop/`

## 说明
- 纯前端单文件，0 依赖；数据存于**各人浏览器 localStorage**（非集中存储）
- 多人同时用、数据需汇总时，需另接后端 + 数据库（原型阶段不要求）
- `?sid=学号` 分享链接示例：`https://<你的用户名>.github.io/greenloop/?sid=2021010123`
