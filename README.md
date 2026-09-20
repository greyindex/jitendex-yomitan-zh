# Jitendex 日中辞典（Yomitan 中文版）

这是一个基于 [Jitendex](https://github.com/Jitendex/Jitendex) 的非官方中文本地化版本，供 Yomitan 使用。

本项目以日文原词条、读音、词性和词条结构为主，英文释义仅作为辅助参考；英文释义和例句已经转换为中文。原始日文内容、图形资源及来源信息均予以保留。

> 这是社区派生版本，不是 Jitendex 官方发布物。Jitendex 官方项目仍然是日英词典。

## 下载与安装

从 [Releases](https://github.com/lzzxccxxzzz/jitendex-yomitan-zh/releases/latest) 下载最新的 `jitendex-yomitan-zh-iq2.zip`，然后在 Yomitan 的 **Dictionaries → Import** 中导入 ZIP 文件。

压缩包的 `index.json` 位于根目录，可以直接导入。该中文版本不包含指向官方英文版本的自动更新地址，因此不会误覆盖官方日英词典。

## 当前版本

- 上游版本：Jitendex 2026-08-11
- 词典文件：218 个 term bank，435,448 个词条
- 已本地化字段：764,036 个
- 图形资源：Jitendex 原始 `graphics` 与 `HanaMinA`
- 翻译模型：本地 Qwen3.8-27B IQ2
- 处理方式：日文优先、英文辅助；模型失败条目已人工补全

## 关键词

Jitendex、Yomitan、Japanese Chinese dictionary、日中辞典、日汉词典、日语中文、日语学习、中文释义。

## 来源与许可

本项目保留上游 Jitendex 的署名和第三方数据说明。详见 [NOTICE.md](NOTICE.md) 与 [LICENSE](LICENSE)。

- 上游项目：[Jitendex/Jitendex](https://github.com/Jitendex/Jitendex)
- Jitendex 网站：[jitendex.org](https://jitendex.org/)
- JMdict 数据：Electronic Dictionaries Research Group
- 日英例句来源：Tatoeba，原始数据按 CC BY 2.0 FR 提供

如发现中文释义、例句或词条结构问题，欢迎提交 Issue，并附上日文词条和上下文。
