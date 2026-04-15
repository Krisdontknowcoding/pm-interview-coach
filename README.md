# PM Interview Coach

通用 PM 面试辅导教练，支持简历分析 + 小红书面经搜索 + 模拟面试 + 参考答案输出。

---

## 功能

- 🎯 **模拟真实面试**：扮演目标公司资深 PM，按一面节奏出题
- 📄 **简历读取**：支持 PDF 路径或文字粘贴，自动提取经历
- 📱 **小红书面经**：搜索 + 读取帖子正文和图片，提取真实面试题
- 🖼️ **图片理解**：用 MiniMax-VL-01 识别截图中的面试题
- 📊 **反馈评估**：整体表现 + 每道题参考答案 + 补充推荐题

---

## 前置要求

- Python 3 + pdfplumber（读取 PDF）
- mcporter 配置好 xiaohongshu MCP 服务
- MiniMax-VL-01 模型（图片理解）

---

## 安装

```bash
# 安装 PDF 依赖
pip3 install pdfplumber pypdf --break-system-packages

# 安装 skill
clawhub install pm-interview-coach --dir ~/.openclaw/skills
```

---

## 使用

触发方式：
- "面试辅导"
- "模拟面试"
- "帮我练习面试"
- "产品经理面试"

**注意：在收集到简历 + 目标公司/岗位 + JD 之前，不会出题。**

---

## 链接

- GitHub: https://github.com/Krisdontknowcoding/pm-interview-coach
- ClawHub: https://clawhub.ai/skills/pm-interview-coach

---

## 更新日志

### v1.1.0
- 新增：面试后提供完整参考答案 + 补充推荐题
- 新增：参考答案格式规范（含加分项/常见错误）
- 修复：强制要求收集简历+岗位+JD后才能出题

### v1.0.0
- 初始版本
- 支持小红书面经搜索 + 面试模拟
- 支持 PDF 简历读取
- 支持 MiniMax-VL-01 图片理解
