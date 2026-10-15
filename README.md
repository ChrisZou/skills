# Skills

创哥的内容创作 skills，包含口播风格指南和小红书标题创作工具。

## 包含的 skills

| Skill | 用途 |
| --- | --- |
| [chuangge-style](chuangge-style/SKILL.md) | 按创哥的语言风格创作或改写视频口播稿，附风格档案和例句。 |
| [xiaohongshu-title-writing](xiaohongshu-title-writing/SKILL.md) | 根据视频脚本生成小红书标题、封面文字及分析，附标题公式、示例和 HTML 模板。 |

## 使用

将需要的 skill 文件夹完整复制到项目的 `.claude/skills/` 目录，保留其中的参考文件：

```text
.claude/skills/
├── chuangge-style/
│   ├── SKILL.md
│   └── chuangge-style.md
└── xiaohongshu-title-writing/
    ├── SKILL.md
    └── references/
```

可使用「用创哥的风格改写这段口播稿」或「根据这个脚本写小红书标题」触发对应 skill。

## 公开版本说明

本仓库仅包含 skill 定义及必要参考资料。个人健康相关表述已泛化；未包含原始脚本、历史生成结果、本地配置或凭据。风格档案中的部分例句经过隐私处理，不作为逐字引用。

生成的 `output/` 目录默认不纳入版本管理。
