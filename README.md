# 交易台练习场 · Trading Desk Practice

为 **CFA Institute × AmplifyME Investing Simulator Challenge** 准备的中文练习模拟器和学习材料。

A Chinese-language practice simulator and study kit for the CFA Institute × AmplifyME Investing Simulator Challenge. Play as an **investment bank** (quote two-way prices, unwind risk on the exchange) or as an **asset manager** (build an ESG-tilted portfolio, react to news, beat the benchmark).

> 这是一个独立的学习项目，与 CFA Institute 和 AmplifyME 没有关联。模拟器里的价格走势、客户行为和佣金都是估计值，不代表官方计分。
> This is an independent study project, not affiliated with CFA Institute or AmplifyME. Prices, client behaviour and fees are simulated estimates, not official scoring.

## 在线试玩

部署后访问：`https://<你的 GitHub 用户名>.github.io/amplifyme-trading-sim/`

## 内容

| 文件 | 内容 |
|---|---|
| `index.html` | 首页 |
| `sim.html` | 练习模拟器 |
| `hub.html` | 交互式学习地图 |
| `docs/intro-course.pdf` | 金融市场入门课程（8 节课） |
| `docs/competition-handbook.pdf` | 比赛日手册 |
| `docs/course-notes.md` | 课程讲义精简版 |
| `docs/asset-manager-playbook.md` | 资管作战手册 |

## 模拟器功能

- **两个角色**：投资银行（IB）、资产管理（AM）
- **两组资产**：比赛同款（RDS、SIE、EDF、TSLA、NVDA，含比赛中出现过的真实新闻）和练习版（BABA、MSFT、VW、HSBC、BP）
- **三种模式**：情景训练（时间暂停，逐步引导）、轻松（节奏减半，询价时自动暂停）、标准
- **盯盘提示**：每个指标标注“越高越好 / 越低越好”，并给出下一步行动；关掉后界面接近真实平台
- **局后复盘**：成绩单、做得好的地方、按时间顺序列出的错误和改进建议、下一局最该注意的三件事
- **中英双语**：界面标签和聊天消息都有中英对照

单个 HTML 文件，不需要安装、不需要后端，打开就能玩。

## 部署到 GitHub Pages

### 方法一：网页上传（不需要命令行）

1. 登录 GitHub，点右上角 **+** → **New repository**，名字填 `amplifyme-trading-sim`，选 **Public**，点 **Create repository**。
2. 在新仓库页面点 **uploading an existing file**，把这个文件夹里的**所有文件和 `docs` 文件夹**一起拖进去，点 **Commit changes**。
3. 进入仓库的 **Settings** → 左侧 **Pages**。
4. **Source** 选 **Deploy from a branch**，**Branch** 选 `main`、文件夹选 `/ (root)`，点 **Save**。
5. 等一两分钟，页面顶部会出现网址：`https://<用户名>.github.io/amplifyme-trading-sim/`。

### 方法二：命令行

```bash
cd amplifyme-trading-sim
git init
git add .
git commit -m "First version"
git branch -M main
git remote add origin https://github.com/<用户名>/amplifyme-trading-sim.git
git push -u origin main
```

然后按方法一的第 3 至 5 步开启 Pages。

## 本地运行

直接用浏览器打开 `index.html` 即可。

## 许可

MIT License，见 `LICENSE`。
