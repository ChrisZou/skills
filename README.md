# Skills

创哥的内容创作 skills，包含口播风格指南、小红书标题创作工具和 davinci 封面制作 skill。

## 包含的 skills

| Skill | 用途 |
| --- | --- |
| [chuangge-style](chuangge-style/SKILL.md) | 按创哥的语言风格创作或改写视频口播稿，附风格档案和例句。 |
| [xiaohongshu-title-writing](xiaohongshu-title-writing/SKILL.md) | 根据视频脚本生成小红书标题、封面文字及分析，附标题公式、示例和 HTML 模板。 |
| [davinci](davinci/SKILL.md) | 通过 davinci CLI 制作和修改封面、管理素材及模板、导出图片；需搭配 [davinci 项目](https://github.com/ChrisZou/davinci) 使用。 |

## 使用

将需要的 skill 文件夹完整复制到项目的 `.claude/skills/` 目录，保留其中的参考文件：

```text
.claude/skills/
├── chuangge-style/
│   ├── SKILL.md
│   └── chuangge-style.md
├── xiaohongshu-title-writing/
│   ├── SKILL.md
│   └── references/
└── davinci/
    ├── SKILL.md
    ├── references/
    ├── examples/
    └── LICENSE
```

可使用「用创哥的风格改写这段口播稿」或「根据这个脚本写小红书标题」触发对应 skill。

## davinci：需搭配 davinci 项目使用

**`davinci` skill 需要搭配 [davinci 项目](https://github.com/ChrisZou/davinci) 使用。** 它通过 `davinci` CLI 操作本地图片编辑器，单独复制 skill 不会安装应用或命令行工具。

1. 按 [davinci README](https://github.com/ChrisZou/davinci#readme) 安装桌面版或从源码运行。
2. 桌面版按首次启动引导安装命令行工具，也可从应用菜单安装；源码版在 davinci 项目目录执行 `./start.sh install` 安装 CLI。安装后新开终端。
3. 将本仓库的 `davinci/` 文件夹完整复制到项目的 `.claude/skills/`，然后新开 Agent 会话。
4. 执行 `davinci projects` 确认可用；返回空项目列表也正常。

之后可以让 Agent「用 davinci 做一张小红书封面，标题是……」，或发给它 davinci 编辑器中的项目链接来修改已有设计。需要人像、Logo 或背景时，使用你自己的素材库。

本目录同步自 davinci 项目的 `skills/davinci/`，使用说明以对应版本的 davinci 文档和 `davinci schema` 为准；示例 JSON 中的素材 URL 需要替换为实际素材。davinci skill 沿用源项目的 [Apache-2.0 许可证](davinci/LICENSE)。

## 公开版本说明

本仓库仅包含 skill 定义及必要参考资料。个人健康相关表述已泛化；未包含原始脚本、历史生成结果、本地配置或凭据。风格档案中的部分例句经过隐私处理，不作为逐字引用。

生成的 `output/` 目录默认不纳入版本管理。
