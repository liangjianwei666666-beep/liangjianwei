# 视觉笔记信息图 Codex Skill

一个用于批量生成中文竖版视觉笔记信息图和生图提示词的 Codex skill。

默认图像规格：

- 手绘扁平矢量插画，视觉引导风格
- 模块化知识地图，干净留白，层级流动
- 中文文字，字体指定为 Ma Shan Zheng
- 高清竖版，1242x1660 像素
- 底部署名默认为 `@自定义 制作`

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

```text
用 $visual-note-infographics 把下面 10 个主题批量生成中文竖版视觉笔记提示词。
```

```text
用 $visual-note-infographics 绘制这 3 张视觉笔记，底部标记改成 @我的账号 制作。
```
