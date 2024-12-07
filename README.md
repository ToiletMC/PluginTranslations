# PluginTranslations

帮助我们改进翻译。

## 翻译规则

- 尽量避免[翻译腔](https://zh.wikipedia.org/wiki/Wikipedia:%E7%BF%BB%E8%AF%91%E8%85%94)。
- 应当保持语句的简洁、清爽，不宜使用过多的颜色代码。
- 如果消息有前缀，请使用 `&8[插件名或相关提示&8]` 格式，例如：`&8[&a领地&8]`。
- CMI 的消息颜色默认是使用 `&e` 的，我们需要使用 `&6`，因为这个颜色不错，而且 [EssentialsX](https://essentialsx.net/) 也在用！
- 【和[Minecraft 官方翻译](https://crowdin.com/editor/minecraft/10038/enus-zhcn?view=comfortable&filter=basic&value=0)风格一致】所有标点符号都应使用中文，包括逗号、句号、感叹号等等。专有名词、数字应该和中文之间最好不要有空格，例如 `你收到了6马桶币！` 。
- 如果翻译的语言是物品的 lore，过长则应该换行展示。

## 词汇表

| 单词 | 翻译 |
| ---- | ---- |
| Land | 领地 |
| ...  | ...  |

## 注意事项

- 所有翻译将在每周的周末或月底同步到服务器。
- 英文翻译是最新的，如果语言文件的字段有出入，以英文语言文件的字段为准。
- 中文翻译更新不太及时，有可能会出现缺少字段、字段变更未及时更新的情况，你可以提一个 PR 解决该问题！

## 目录结构

此仓库中的 `translations` 文件夹直接对应了服务器上的 `plugins` 文件夹。

## 工作流介绍

当 `translations` 文件夹有更新时，会运行工作流 `apply.yml`。

此工作流会将 `translations` 文件夹中的所有语言文件上传到服务器的 `plugins` 文件夹中，等待服务器在夜间重启时生效。
