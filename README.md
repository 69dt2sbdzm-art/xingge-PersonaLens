# 好玩的人类观察计划 - MBTI匹配分析工具

一个基于荣格心理类型理论的MBTI人格分析小程序，提供16种人格类型的深度探索、关系匹配和对比分析功能。

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Taro](https://img.shields.io/badge/Taro-4.2.0-green.svg)
![React](https://img.shields.io/badge/React-18.0-blue.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-5.4-blue.svg)

## ✨ 功能特性

### 🔍 探索页 - 16种人格类型详解
- **四大类别分组**：分析家(NT)、外交家(NF)、守护者(SJ)、探险家(SP)
- **完整认知功能栈**：主导功能到劣势功能的详细解析
- **多维核心优势**：思维维度、工作风格、人际互动、创造力
- **潜在盲区与改进建议**：识别弱点并提供成长方向
- **关系洞察**：亲密关系、友谊模式的深度分析
- **职业发展指南**：最佳职业、工作风格、理想环境
- **典型代表人物**：带可信度评级的真实案例

### 💕 匹配页 - 关系兼容性分析
- **智能匹配度计算**：基于四维度加权算法（S/N 35%、T/F 25%、E/I 20%、J/P 20%）
- **工作兼容性评估**：协作优势、潜在摩擦、实践建议
- **感情火花值分析**：情感共鸣、吸引力因素、深化建议
- **视觉化展示**：发光渐变进度条 + 动态特效（小花🌸/爱心❤️）
- **分级颜色系统**：
  - <60%：亮黄色（需要磨合）
  - 60-80%：淡橙色 + 小花特效（良好匹配）
  - ≥80%：粉色 + 爱心特效（绝佳搭档）

### ⚖️ 比较页 - 双类型对比分析
- **概述对比**：核心特质并排展示
- **认知功能对比表**：功能栈差异一目了然
- **核心优势对比**：四维优势横向比较
- **潜在盲区对比**：弱点分析与互补性
- **推荐职业方向**：适合的职业领域并列展示

## 🛠️ 技术栈

- **框架**：[Taro 4.x](https://taro.zone/) - 跨端小程序开发框架
- **UI库**：React 18 + TypeScript
- **样式**：Tailwind CSS v4 + 玻璃拟态设计(Glassmorphism)
- **状态管理**：Zustand
- **图标**：Lucide Icons + Material Design Icons
- **包管理器**：pnpm

## 📦 快速开始

### 前置要求
- Node.js >= 18
- pnpm >= 9.0

### 安装依赖
```bash
pnpm install
```

### 开发模式
```bash
# H5预览（默认端口3015）
pnpm run dev

# 微信小程序开发
pnpm run dev:weapp
```

### 构建生产版本
```bash
# 微信小程序构建
pnpm run build

# H5构建
pnpm run build:web
```

### 代码校验
```bash
pnpm run validate
```

## 📁 项目结构

```
├── src/
│   ├── pages/              # 页面目录
│   │   ├── explore/        # 探索页 - 16种人格类型
│   │   ├── match/          # 匹配页 - 关系兼容性
│   │   └── compare/        # 比较页 - 双类型对比
│   ├── components/         # 可复用组件
│   ├── data/               # 数据文件
│   │   └── mbti-types.ts   # 16种人格完整数据
│   ├── lib/                # 工具函数
│   │   └── mbti-match.ts   # 匹配度计算算法
│   ├── api/                # API接口
│   └── store/              # 状态管理
├── config/                 # 配置文件
├── functions/              # Edge Functions
└── dist/                   # 构建产物
```

## 🧮 匹配度算法说明

### 理论基础
- **荣格心理类型理论** (Jungian Cognitive Functions)
- **认知功能栈理论** (Cognitive Function Stack)
- **类型动力学** (Type Dynamics)

### 权重分配
| 维度 | 权重 | 说明 |
|------|------|------|
| S/N | 35% | 决定认知世界的根本方式，最重要 |
| T/F | 25% | 影响决策方式和沟通效率 |
| E/I | 20% | 能量来源，可通过适应协调 |
| J/P | 20% | 生活节奏，相对次要 |

### 特殊处理
- **同类型配对**：95分（非100分，承认缺乏互补性）
- **工作兼容性**：J/J相同+5分，T/T相同+3分
- **感情火花值**：N/N+8分，E/I互补+5分，F/F+6分，S/S-3分

## 🎨 设计特色

- **玻璃拟态风格**：backdrop-blur + 半透明背景 + 柔和阴影
- **四大类别视觉区分**：紫色(分析家)、绿色(外交家)、蓝色(守护者)、橙色(探险家)
- **统一emoji图标**：每种类型都有符合特质的专属图标
- **流畅动画效果**：CSS关键帧动画实现粒子浮动
- **响应式布局**：适配不同屏幕尺寸

## 📱 平台支持

- ✅ 微信小程序
- ✅ H5网页
- 🔄 其他小程序平台（需额外配置）

## 🤝 贡献指南

欢迎提交Issue和Pull Request！

1. Fork本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🙏 致谢

- [Myers & Briggs Foundation](https://www.myersbriggs.org/) - MBTI官方理论
- [Personality Hacker](https://personalityhacker.com/) - 认知功能栈理论
- [TypeLogic](https://www.typelogic.com/) - 类型动力学研究

---

**Made with ❤️ by 好玩的人类观察计划团队（星舸）**
