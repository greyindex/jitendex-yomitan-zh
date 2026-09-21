# Jitendex 日中辞典（Yomitan 中文版）

这是一个基于 [Jitendex](https://github.com/Jitendex/Jitendex) 的非官方中文本地化版本，供 Yomitan 使用。

本项目以日文原词条、读音、词性和词条结构为主，英文释义仅作为辅助参考；英文释义和例句已经转换为中文。原始日文内容、图形资源及来源信息均予以保留。

> 这是社区派生版本，不是 Jitendex 官方发布物。Jitendex 官方项目仍然是日英词典。

## 下载与安装

从 [Releases](https://github.com/lzzxccxxzzz/jitendex-yomitan-zh/releases/latest) 下载最新的 `jitendex-yomitan-zh-common5pct-luna.zip`，然后在 Yomitan 的 **Dictionaries → Import** 中导入 ZIP 文件。

压缩包的 `index.json` 位于根目录，可以直接导入。该中文版本不包含指向官方英文版本的自动更新地址，因此不会误覆盖官方日英词典。

本版词典标题为「Jitendex.org [2026-08-11] 中文版 常用5%校订版」。已安装旧中文版的用户，导入后可停用旧版以避免重复显示；[初版](https://github.com/lzzxccxxzzz/jitendex-yomitan-zh/releases/tag/v2026.08.11-zh.1)仍可下载。

## 当前版本

- 发布版本：`v2026.08.11-zh.2`（2026-09-21，常用 5% 二次校订）
- 上游版本：Jitendex 2026-08-11
- 词典文件：218 个 term bank，435,448 条记录（含变体和重定向），211,107 个不同 JMdict 词条 ID
- 已本地化字段：764,036 个
- 图形资源：Jitendex 原始 `graphics` 与 `HanaMinA`
- 翻译模型：本地 Qwen3.8-27B IQ2
- 处理方式：日文优先、英文辅助；模型失败条目已额外补全

## 第二次校对结果

按 Jiten Global 2026-09-19 词频匹配，选取 **10,556 个常用词候选（约占词条 ID 的 5%）**，由 GPT-5.6 Luna 并行校对入选词的全部释义、例句和辅助说明。

- 审读 **86,698 个去重字段**，覆盖 17,272 条释义变体记录。
- 修正 **1,598 个唯一字段**；展开到重复变体后共 **2,222 处修改**，涉及 **1,044 个词条 ID**。
- **5 个字段、3 个词条仍待核实**，保留原译并公开列出。
- 全部 435,448 条记录通过结构对比；ZIP 的 471 个文件通过 CRC 和逐文件哈希检查，原日文、读音、图片、标签和署名保留。

详见[第二轮校对报告](reports/2026-09-21/SECOND_PASS.md)、[修正明细](reports/2026-09-21/corrections.csv)、[待核实清单](reports/2026-09-21/uncertain.csv)及[入选词表](reports/2026-09-21/common_top_5pct.csv)。下载文件可使用 [SHA256SUMS.txt](SHA256SUMS.txt) 核对。

## 仍然存在的问题

- **长尾及未入选词条没有经过本轮语义校对**，仍可能存在原模型的错义、术语误译、遗漏或不自然表达。
- 已知疑点包括「体感」的 3 个专业术语字段、「ミス」与英文 `myth` 的对应，以及「無条件」例句的日英含义冲突。它们是待核事项，不都能直接认定为翻译错误。
- 常用 5% 是基于所选语料与词形匹配的候选范围，并非义项级的绝对频率排名；422 个入选 ID 涉及同形同音歧义，另有 39,506 个词条未匹配词频，不能据此断言为低频。
- 本轮是模型校对，**没有重新测得修正后的全库误译率，也不保证已校对字段零错误**。结构检查通过仅说明数据完整性，不代表语义准确率。

## 关键词

Jitendex、Yomitan、Japanese Chinese dictionary、日中辞典、日汉词典、日语中文、日语学习、中文释义。

## 来源与许可

本项目保留上游 Jitendex 的署名和第三方数据说明。详见 [NOTICE.md](NOTICE.md) 与 [LICENSE](LICENSE)。

- 上游项目：[Jitendex/Jitendex](https://github.com/Jitendex/Jitendex)
- Jitendex 网站：[jitendex.org](https://jitendex.org/)
- JMdict 数据：Electronic Dictionaries Research Group
- 日英例句来源：Tatoeba，原始数据按 CC BY 2.0 FR 提供

如发现中文释义、例句或词条结构问题，欢迎提交 Issue，并附上日文词条和上下文。
