# 平时大作业三 · 作品集

聚合课堂作业六至八的全部成果，统一入口运行。

## 项目简介

六个模块，覆盖完整前端技术栈：

| 模块 | 文件 | 演示内容 | 来源 |
| --- | --- | --- | --- |
| 1. jQuery | `1-jquery-filter.html` | 自习室楼层 + 状态筛选 | lecture8/integration |
| 2. 异步加载 | `2-async-dashboard.html` | fetch + try/catch + 三态提示 | homework6/my-dashboard |
| 3. ECharts | `3-echarts-rockets.html` | 分组柱状图 + itemStyle 高亮 | lecture8/rockets |
| 4. Chart.js | `2-async-dashboard.html` | 折线图 + responsive | homework6/my-dashboard |
| 5. Three.js | `4-three-js.html` | 五件套 + OrbitControls | lecture7/three-d |
| 6. A-Frame | `5-a-frame-rockets.html` | 鼻锥+箭体+喷嘴+火焰 | lecture8/rockets |

## 运行方式

```bash
cd total-3
python3 -m http.server 8000
# 浏览器打开 http://localhost:8000/
```

或用 VS Code 的 Live Server 打开 `index.html`。

## 目录说明

```
total-3/
├── index.html              作品集首页（6 模块卡片）
├── 1-jquery-filter.html
├── 2-async-dashboard.html
├── 3-echarts-rockets.html
├── 4-three-js.html
├── 5-a-frame-rockets.html
├── css/style.css
├── libs/                   所有库（bootstrap/jquery/echarts/chart.js/aframe/three.js）
├── data/                   共享 JSON（library/rockets/study-rooms）
└── README.md
```

## 库与资源来源

| 库 | 来源 |
| --- | --- |
| Bootstrap | [getbootstrap.com](https://getbootstrap.com/) |
| jQuery 3.7.1 | [jquery.com](https://jquery.com/) |
| ECharts | [echarts.apache.org](https://echarts.apache.org/) |
| Chart.js | [chartjs.org](https://www.chartjs.org/) |
| Three.js + OrbitControls | [threejs.org](https://threejs.org/) |
| A-Frame | [aframe.io](https://aframe.io/) |

各 demo 的代码来源：
- jQuery 筛选：lecture8/integration/study-rooms.html
- 异步看板：homework6/my-dashboard
- ECharts 火箭：lecture8/rockets/detail.html（itemStyle.color 按数据点覆盖 trick）
- Three.js 展示台：lecture7/three-d/showcase.js（简化版）
- A-Frame 火箭：lecture8/rockets/three-d/scene.html

数据文件均为模拟数据：
- `data/library.json` —— 借阅数据
- `data/rockets.json` —— 4 个火箭参数
- `data/study-rooms.json` —— 自习室信息