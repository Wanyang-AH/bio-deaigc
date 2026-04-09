# bio-deaigc

生物信息学领域中文学术文本去 AIGC 润色工具，基于 [Claude Code Skills](https://docs.anthropic.com/en/docs/claude-code/skills) 构建。

## 简介

当用户提供生物信息学、基因组学、转录组学、蛋白质组学、多组学分析、流程开发（pipeline）、云平台部署等方向的中文学术文本时，本 skill 可对其进行"去 AI 化"重写，使文本读起来更像真人撰写。

适用场景：

- 学位论文 / 开题报告段落润色
- 简历中的项目描述改写
- 期刊投稿文本降 AIGC 率

## 安装

### 前提条件

- 已安装 [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview)

### 安装步骤

在终端中运行：

```bash
claude install-skill https://github.com/Wanyang-AH/bio-deaigc
```

安装后，skill 会自动注册到你的 Claude Code 环境中，无需额外配置。

## 使用方法

安装后无需手动调用。当你在 Claude Code 中输入生物信息学相关的中文文本并使用以下触发词时，skill 会自动触发：

> 去 AI 味、去 AIGC、润色、降重、改写、人话、自然一点、学术化……

即使只说"帮我改一下这段话"，只要内容涉及生物信息学，也会自动触发。

也可以通过斜杠命令手动调用：

```
/bio-deaigc
```

## 核心能力

- 识别并替换空洞渲染词（如"深入挖掘" → "分析"）
- 修正翻译腔长定语句式
- 消除机械列举、被动语态堆砌等 AI 痕迹
- 保护生信领域专有术语不被误改（GATK、DESeq2、WGCNA 等）
- 输出纯文本，符合国内期刊排版规范

## 示例

**输入：**

> 随着高通量测序技术的蓬勃发展，生物信息学应运而生，为深入挖掘海量组学数据提供了强有力的工具，在精准医学领域具有不可或缺的重要地位。

**输出：**

> 高通量测序技术的发展推动了生物信息学在组学数据分析中的广泛应用，目前已成为精准医学研究的重要方法。

## 许可证

[MIT](LICENSE)
