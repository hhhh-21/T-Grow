# 鹅伴 T-Grow｜AI 求职成长陪伴助手 Demo

这是一个面向在校大学生的 AI 求职成长陪伴产品 Demo。产品根据学生年级、专业、兴趣、经历和困惑，生成：

- 当前成长阶段诊断
- 腾讯相关岗位兴趣方向 Top 3
- 能力差距分析
- 30 天成长计划
- 今日行动建议
- 求职问答
- 简历经历转化

> 注意：本 Demo 使用模拟岗位库与规则生成逻辑，不代表腾讯官方岗位开放情况或录用标准。可选配置 OpenAI API Key 后启用大模型生成。

## 本地运行

```bash
pip install -r requirements.txt
streamlit run app.py
```

## 启用大模型生成（可选）

在 Streamlit Community Cloud 的 Secrets 中添加：

```toml
OPENAI_API_KEY="你的 OpenAI API Key"
```

也可以本地设置环境变量：

```bash
export OPENAI_API_KEY="你的 OpenAI API Key"
```

## 部署

推荐使用 Streamlit Community Cloud：

1. 新建 GitHub 仓库，例如 `tgrow-demo`
2. 上传本项目所有文件
3. 进入 Streamlit Community Cloud
4. 选择仓库、分支和入口文件 `app.py`
5. 点击 Deploy
6. 获取公网访问链接

## 项目结构

```text
.
├── app.py
├── requirements.txt
├── README.md
├── DEPLOY_WITH_CODEX.md
└── .streamlit/
    └── config.toml
```
