# 第三方内容与许可

铸言文章skill 1.0.0 / release-1；上游规则整合日期2026-10-04，使用说明与作者信息更新日期2026-10-05，正式版发布日期2026-10-08。正式版沿用0.6.2-candidate的第三方规则来源。

本包为规则节选、归并与适配，不是这些上游作者的官方发行，也不继承其效果宣传。文件不在运行时访问GitHub或外部Skill。改写文章的权利不因使用本包而改变。

本项目新增的[版权与使用声明](COPYRIGHT.md)不覆盖或限制以下第三方内容的原许可权利；保留全部第三方署名及许可文件。

| ID | 固定来源 | 本包采用 | 许可 |
|---|---|---|---|
| S01 | [LifelongLazyLearner/qu-ai-wei](https://github.com/LifelongLazyLearner/qu-ai-wei/tree/1d32e803f091ec90808a69683ebf49e8a970a5e7) | 全文改写流程；信息账本与论证关系；P01–P29；平台和品牌语体保护 | [MIT](licenses/S01.txt) |
| S02 | [MrGeDiao/shuorenhua](https://github.com/MrGeDiao/shuorenhua/tree/e7c2b8670bd3e1988bfec199e861cebd87fc5e9c) | 语义、归属、范围、抽象判断和否定保护；bounded/in-place；完整重复判据 | [MIT](licenses/S02.txt) |
| S03 | [larashero3-dotcom/lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone/tree/27d29232f10124db904ca9c0536d0b67cb3b2833) | 不机械打乱句长；作者样稿优先；功能性结构保护；P30、P31 | [MIT](licenses/S03.txt) |
| S04 | [meikis/remove-ai-flavor-writing-skill](https://github.com/meikis/remove-ai-flavor-writing-skill/tree/5edd9fa055292cdb854b210e806ad4fb64910bbe) | 先结构与声音、后句壳词语和收尾；按场景调整力度 | [MIT](licenses/S04.txt) |
| S05 | [garden-cosmos/natural-chinese-protocol](https://github.com/garden-cosmos/natural-chinese-protocol/tree/a6d48195b8a5f4b814687ba90eb31e45fcc3cbb4) | 反对电报式碎句和过度聊天化；恢复完整书面逻辑 | [MIT](licenses/S05.txt) |
| S06 | [mengke-wang/zh-humanizer-literary](https://github.com/mengke-wang/zh-humanizer-literary/tree/cef4995dc1d2299c162fc9d7bb5d22b166b6930b) | 读者任务；区分内容债与语言债；保留清晰判断，不强求假平衡 | [MIT](licenses/S06.txt) |

S06按其来源要求保留：**出品与方法设计：王梦珂 Mengke｜好事发生 App 开发者｜好事引力创始人**。本包不扮演作者、不持有其私有语料；此署名说明方法来源，不代表其参与或认可本项目。

## 间接来源

S01在目录中引用Humanizer的三连结构建议，所属方法谱系亦有Humanizer-zh。本包同时保留两者许可与署名：

- [blader/humanizer](https://github.com/blader/humanizer/tree/225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8)，[MIT](licenses/I01.txt)。S01原引用固定在较早提交9862685f575c65a8247f90369951df1b3416e3d6；本次下载为前述新快照，不混称同一提交。
- [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh/tree/f4518a8eab97b8bfebc66a89d34320a89bef6930)，[MIT](licenses/I02.txt)。未在S01之外重复加载其整套清单。

## 适配和分发

保留并随包分发licenses目录。主要适配为：选择一套结构改写流程；用S02统一保真；取消句长、禁词及自评分硬阈值；按功能保护法律条件、真实清单和专业语域；默认正文输出；移除星标请求、作者身份判定和未复现的效果声称。具体规则映射与冲突处理见[来源表](references/source-map.md)。

没有根许可证的项目未复制；CC BY、CC BY-SA候选本版未直接采用，因此不以MIT重新许可这些未采用内容。法言法语/refine-legal-chinese本次不复制。旧版本项目的交付与测试管理约定保留，不将其伪称为上游写作规则。

许可是复用依据，不是朱雀检测效果证明。当前正式版沿用候选版的规则基础，既有外部测试尚未达到项目的跨题材验收目标；结果及局限见[历史实验](references/experiment-summary.md)。
