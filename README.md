# 同花损

> 一个股票后悔计算器：输入买入记录，看看如果当初没有卖，或者刚好卖在历史高点，本可以多赚多少钱。

在线体验：[https://regret-market.vercel.app/](https://regret-market.vercel.app/)

## Features

- 支持美股、A 股、港股搜索与计算
- 支持按股数或买入金额输入
- 对比实际卖出收益、继续持有收益、历史高点收益
- 展示价格走势图，并标注买入点、卖出点和历史高点
- 根据错过收益率生成 meme 文案和心痛指数
- 支持生成分享图和复制分享文案
- 使用 Vercel Serverless Functions 代理股票数据接口

## Tech Stack

- HTML / CSS / JavaScript
- Vercel Serverless Functions
- Tushare Pro
- Yahoo Finance chart API
- Canvas API
- html2canvas

## Local Development

```powershell
npx vercel dev
```

本地运行前需要创建 `.env.local`：

```env
TUSHARE_TOKEN=your_tushare_token_here
```

不要把真实 token 写进代码、README 或提交到 GitHub。

## Deployment

推荐使用 Vercel 免费方案部署。

在 Vercel 项目中配置环境变量：

```env
TUSHARE_TOKEN=your_tushare_token_here
```

然后推送到 GitHub，Vercel 会自动重新部署。

## Project Structure

```text
.
├── index.html
├── api
│   ├── stock.js
│   └── search.js
├── stocks-data
├── vercel.json
├── package.json
└── README.md
```

## Contributors

- [Yuzhao](https://github.com/crake7even)

## Author

**Yuzhao**

- GitHub: [crake7even](https://github.com/crake7even)
- 小红书: [Yuzhao](https://xhslink.com/m/3DzxhFipyIc)

## License

MIT
