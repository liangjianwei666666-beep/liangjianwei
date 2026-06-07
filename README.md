# 视觉笔记信息图 Codex Skill

一个用于批量生成中文竖版视觉笔记信息图和生图提示词的 Codex skill。适合把文章观点、课程知识、心理学概念、咨询科普、方法论框架和社媒选题，快速转成“模块化知识地图”式的视觉笔记。

它的核心目标不是做复杂海报，而是把抽象内容提炼成清晰的视觉隐喻：少文字、强结构、有留白，让读者一眼看见重点和阅读路径。

## 适合做什么

- 中文视觉笔记信息图
- 小红书/公众号/知识卡片配图
- 课程、咨询、心理学、方法论内容的概念图
- 批量生图提示词
- 连续主题系列图，比如“5 个阶段”“7 个步骤”“3 个误区”
- 带固定署名的品牌化内容图

## 默认图像规格

- 手绘扁平矢量插画，视觉引导风格
- 模块化知识地图，干净留白，层级流动
- 中文文字，字体指定为 Ma Shan Zheng
- 高清竖版，1242x1660 像素
- 底部署名默认为 `@自定义 制作`
- 强调复杂理念的视觉综合，而不是长文堆叠

## 一键安装

在 Codex 中输入：

```text
Use $skill-installer to install https://github.com/liangjianwei666666-beep/liangjianwei/tree/main/skills/visual-note-infographics
```

如果你的 Codex 支持 skill installer，它会从 GitHub 下载并安装这个 skill。

也可以在本机运行：

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo liangjianwei666666-beep/liangjianwei \
  --path skills/visual-note-infographics
```

安装完成后，重启 Codex 以加载新 skill。

## 使用示例

批量生成提示词：

```text
用 $visual-note-infographics 把下面 10 个主题批量生成中文竖版视觉笔记提示词。
```

直接生成图片：

```text
用 $visual-note-infographics 绘制这 3 张视觉笔记，底部标记改成 @我的账号 制作。
```

连续系列内容：

```text
用 $visual-note-infographics 批量生成 5 张信息图：心理咨询的五个阶段，连续的信息内容，写明由 @在地心理 制作。
```

总览总结页：

```text
用 $visual-note-infographics 给这组内容再生成一张总概括信息图，提炼核心要义即可。
```

## 生成逻辑

每张图会先把内容压缩成：

- 一个中心隐喻
- 3-6 个知识模块
- 一条清晰的视线流动路径
- 4-10 个短中文标注词

再按视觉笔记风格生成完整提示词或图片。这样可以避免常见的信息图问题：字太多、像 PPT、模块混乱、只有装饰没有认知结构。

## 输出口径

默认生成的是竖版中文图，适合手机端阅读和社媒发布。如果你只需要提示词，可以明确说“只输出提示词”；如果要直接出图，可以说“生成图片”或“绘制”。

## 仓库结构

```text
skills/visual-note-infographics/
├── SKILL.md
└── agents/openai.yaml
```

这个仓库的 skill 入口是：

```text
https://github.com/liangjianwei666666-beep/liangjianwei/tree/main/skills/visual-note-infographics
```
