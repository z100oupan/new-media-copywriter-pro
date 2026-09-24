# 新媒体运营文案 Pro

面向中文新媒体运营、内容运营和品牌运营的 Codex Plugin，覆盖小红书、抖音、微信公众号、校园内容、品牌 Campaign、韩娱、美食、运营复盘和作品集文案。

## 功能

- 原文润色、去 AI 味和平台改写
- 小红书、抖音、微信公众号内容创作
- 标题、Hook、字幕和 CTA 优化
- 校园活动、品牌内容和活动海报文案
- 运营作品集、简历项目描述和数据复盘
- 信息不足时使用【待补充】，不编造数据、价格、时间、地点和项目成果

## 安装

### 通过 Codex Plugin Marketplace

```bash
codex plugin marketplace add z100oupan/new-media-copywriter-pro --sparse .agents/plugins
codex plugin add new-media-copywriter-pro@new-media-copywriter-pro
```

安装后重启 Codex，或新建一个任务。

### 直接使用 Skill

也可以只使用其中的 Skill：

```bash
git clone https://github.com/z100oupan/new-media-copywriter-pro.git
```

然后把下面目录复制到自己的用户级或项目级 Skill 目录：

```text
skills/new-media-copywriter-pro
```

用户级目录示例：

```text
C:\Users\<用户名>\.codex\skills\new-media-copywriter-pro
```

项目级目录示例：

```text
<项目目录>\.agents\skills\new-media-copywriter-pro
```

## 使用

显式调用：

```text
$new-media-copywriter-pro 帮我写一篇小红书探店文案，保留真实感，不编造价格和地址。
```

也可以自然描述任务：

```text
用新媒体运营文案润色器，帮我把下面这段文案去 AI 味，保留我的语气。
```

## 目录结构

```text
.
├── .agents/
│   └── plugins/
│       └── marketplace.json
├── .codex-plugin/
│   └── plugin.json
├── plugin.json
└── skills/
    └── new-media-copywriter-pro/
        ├── SKILL.md
        ├── references/
        ├── assets/
        └── agents/
```

## 更新

插件源码更新后：

```bash
git add .
git commit -m "Update new-media-copywriter-pro"
git push
```

## 原则

优先保留用户原意和真实信息，不编造数据，不夸大效果，并尽量降低 AI 腔。