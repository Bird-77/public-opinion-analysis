舆情分析平台 🔍

一个轻量级的舆情分析可视化网站，支持关键词搜索和多维度数据分析。

功能特性

情感分析：自动识别正面/中性/负面情感分布
声量趋势：近7天内容发布趋势可视化
热词云图：关键词热度分布展示
平台对比：B站 vs 抖音数据对比
热门内容：按互动量排序的内容列表

技术栈
Vue 3 (CDN)
ECharts 5 (CDN)
纯前端，无需后端

快速开始
下载 index.html 文件
双击打开即可使用
输入关键词，点击"开始分析"

使用说明
演示模式
默认开启，使用模拟数据进行演示。
API模式（可选）


关闭"演示模式"后，会调用后端API获取真实数据。需要自行搭建后端服务，接口格式：

javascript
POST /api/sentiment-analysis
Content-Type: application/json

Request:
{
  "keyword": "搜索关键词",
  "platform": "all" | "bilibili" | "douyin"
}

Response:
{
  "posts": [...],
  "trendData": [...],
  "hotWords": [...],
  "bilibiliData": {...},
  "douyinData": {...},
  "sentimentCounts": {...}
}

部署
GitHub Pages

上传 index.html 到仓库
在仓库 Settings -> Pages 选择分支
访问 https://你的用户名.github.io/仓库名/
Vercel / Netlify


直接拖拽 index.html 文件即可部署。


作者 bird-77
