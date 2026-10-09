# 来源与冲突处理

版本：0.6.0-candidate / upstream-assembly-1。整合审阅：2026-10-04。

本来源映射继续适用于0.6.1-candidate / usage-author-1：该修订仅增加用户提问示例、作者咨询提示和自有内容版权说明，未修改上游编辑模式及第三方许可。

0.6.2-candidate / eval-baseline-1仅根据R10/R11实测收紧检测反馈和基线要求，不改变上游编辑模式、来源映射或第三方许可。此版后来用于R11-v2同题复测，结果未达标；见[历史实验](experiment-summary.md)。

1.0.0 / release-1将上述规则作为首个正式版发布，没有新增第三方来源，也没有把版本升级解释为朱雀效果达标。

这是开发审计，不是写稿时必读文件。源内容被作为待审阅材料；没有运行源脚本、安装源插件、发送文章或执行源文要求的GitHub点赞。

## 直接采用的六个来源

全部为已读取的本地固定提交快照；六个LICENSE正文均核对为MIT，原文许可随包保存在licenses目录。

| ID | 仓库及固定提交 | 采用部分 | 原路径 |
|---|---|---|---|
| S01 | [LifelongLazyLearner/qu-ai-wei](https://github.com/LifelongLazyLearner/qu-ai-wei/tree/1d32e803f091ec90808a69683ebf49e8a970a5e7) · `1d32e803f091ec90808a69683ebf49e8a970a5e7` | 全文改写流程；信息账本与论证关系；P01–P29；平台和品牌语体保护 | SKILL.md；references/pattern-catalog.md；references/editing-boundaries.md；references/platform-patterns.md；references/brand-voice.md；references/whitelists.md |
| S02 | [MrGeDiao/shuorenhua](https://github.com/MrGeDiao/shuorenhua/tree/e7c2b8670bd3e1988bfec199e861cebd87fc5e9c) · `e7c2b8670bd3e1988bfec199e861cebd87fc5e9c` | 语义、归属、范围、抽象判断和否定保护；bounded/in-place；完整重复判据 | SKILL.md |
| S03 | [larashero3-dotcom/lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone/tree/27d29232f10124db904ca9c0536d0b67cb3b2833) · `27d29232f10124db904ca9c0536d0b67cb3b2833` | 不机械打乱句长；作者样稿优先；功能性结构保护；P30、P31 | SKILL.md |
| S04 | [meikis/remove-ai-flavor-writing-skill](https://github.com/meikis/remove-ai-flavor-writing-skill/tree/5edd9fa055292cdb854b210e806ad4fb64910bbe) · `5edd9fa055292cdb854b210e806ad4fb64910bbe` | 先结构与声音、后句壳词语和收尾；按场景调整力度 | SKILL.md |
| S05 | [garden-cosmos/natural-chinese-protocol](https://github.com/garden-cosmos/natural-chinese-protocol/tree/a6d48195b8a5f4b814687ba90eb31e45fcc3cbb4) · `a6d48195b8a5f4b814687ba90eb31e45fcc3cbb4` | 反对电报式碎句和过度聊天化；恢复完整书面逻辑 | SKILL.md |
| S06 | [mengke-wang/zh-humanizer-literary](https://github.com/mengke-wang/zh-humanizer-literary/tree/cef4995dc1d2299c162fc9d7bb5d22b166b6930b) · `cef4995dc1d2299c162fc9d7bb5d22b166b6930b` | 读者任务；区分内容债与语言债；保留清晰判断，不强求假平衡 | skills/zh-humanizer-literary/SKILL.md |

S01主入口和六份引用文件全部审阅，其中examples.md仅作反例检查，未搬入运行包。S02–S06本次采用范围为上表所列已读文件，不表示已审计这些仓库的每个脚本和评测资料。

## 规则追溯与唯一入口

| 本包位置 | 对应上游 | 合并方式 |
|---|---|---|
| SKILL.md 工作模式、全文流程 | S01 确定授权／执行完整重写 | 去掉作者身份门检和强制报告；默认仅正文；用户指定范围优先 |
| fidelity-and-scope.md | S01 仲裁顺序、editing-boundaries；S02 保住什么／编辑范围／来源不明 | 语义保护只在此集中裁决；目录的保护条件保留用于局部判断 |
| P01–P05 内容 | S01 pattern-catalog §1 | 不允许“缺来源就自行收窄”；以S02来源保护替换 |
| P06–P08 推论 | S01 §2 | 保留作者主张；表达修改与实质纠错分开 |
| P09–P12 篇章 | S01 §3；S04 编辑顺序 | 同类开篇、分层和收束只保留一个规则入口 |
| P13–P15 句法 | S01 §4；S03 §10–11；S05 | 主干清楚优先；不是强制短句、主动句、少标点 |
| P16–P19 词汇 | S01 §5；S02 | 完整重复才合并；术语及不同类型限定保护 |
| P20–P23 修辞 | S01 §6；S03 防误伤规则 | 删除“单次对称也必须改”“三项必须拆开”的强制倾向；不测句长配额 |
| P24–P27 体裁 | S01 §7；S03、S04、S05 | 依文章用途选择，不把某个平台腔用于全文 |
| P28–P29 来源 | S01 §8；S02 | 来源跟随被支持陈述；不虚构补齐；不暗中改窄原主张 |
| P30 完美工具人格 | S03 §7 拟人化“好人”比喻 | 仅在遮住实际功能时处理；作者评价和能力断言不能丢 |
| P31 段首无指向评论 | S03 §11 | 指代不清时恢复主体；与P14指代明确时省主语分流 |
| genre-and-voice.md | S01 platform-patterns／brand-voice；S03–S06 | 依使用场景按需读取；不加载源作者人设 |
| 实验与文件版本约定 | 本项目既有用户要求 | 非新增写作规则；只用于诚实交付与外部验收 |

S01目录中研究标签及论文结论没有作为本包的效果证据搬运。本包未复现这些研究，也未证明规则能够改变朱雀分类。目录的29项经适配保留，另加S03的两项非重复信号，共31项；流程和边界不再拆成另一套计数。

## 冲突裁决

| 上游分歧或风险 | 本版采用 |
|---|---|
| S01允许全文重组；S02/S03偏原位轻改 | 去AI味/重写采用结构模式；润色及明确保护范围采用轻改。允许重组不允许丢信息 |
| 打乱长短句 vs S03反对句长操控 | 只改理解和推进受阻的句群，不设长短比例、词频上限或随机停顿 |
| 泛化缺细节就补场景 vs 语义保真 | 只恢复已有细节；材料不足稿外提示，不能编人、时间、经历、数据 |
| 删除强评价/副词 vs 保留作者判断 | 保留方向、程度和效果；只删不承载信息的包装 |
| 不用“不是而是” vs 真实纠错和范围排除 | 按实际关系判断；两端含义均保留，不禁句型 |
| 删结尾/编号/排比 vs 操作与导航功能 | 有独有结论、行动、法定条件或导航用途时保留 |
| 删除模糊归属或收窄范围 vs 不改证据归属 | 保留归属和主张，缺来源稿外提示；实质纠错另外处理 |
| 自然等于口语 vs S05保留完整书面句法 | 正式文本保留语域，合并无功能碎句；不默认朋友聊天 |
| 默认不查外部事实 vs 必要高风险核验 | 只查必要高风险/动态疑点，遵循宿主要求，不扩成全量审查 |
| 强制门检、评分、报告、点赞 | 不纳入正文或自动操作；默认一份可测试正文 |

未搬入上游examples：部分示例会改变否定强度、丢清单项目、增写亲历或推测事实。方法条目以本包保真约束为准，不能照这些例句改写。没有因上游声称“实测有效”而填入本包检测成绩。

## 其他14个候选的筛选结果

以下是下载后的分层筛选，不声称逐行审完全部源码。无独有增量或许可不清即不进入运行包，避免把20套指令并排塞给模型。

| 仓库 | 本次阅读深度 | 决定 |
|---|---|---|
| op7418/Humanizer-zh | 入口结构、许可与既有版本对照 | 通用模式已由S01覆盖；保留间接来源署名，不另叠一套清单 |
| blader/humanizer | 入口结构与许可；核对S01引用 | S01三连模式的间接来源；不再直接引入整份英文规则 |
| hardikpandya/stop-slop | 入口结构与既有整合记录对照 | 新包由S01接管重复/空泛/收尾；不保留另一套禁词及自评分 |
| jiji262/humanizer-chinese | 仓库、分叉与文件结构 | 衍生线索，不当成新的独立方法；不再重复整包引入 |
| Hyacehila/humanizer-zh-next | 主入口分段审阅，未审完全部引用 | 与核心高度重合；固定段落数、拟造个人细节和评分不采用 |
| baibanbao/qu-ai-wei | 主入口分段与冲突部分；未审计全部引用 | 引用了同源材料，核心已覆盖；不继承私人语料依赖和改意示例 |
| Wechat-ggGitHub/chinese-ai-humanizer | 主入口全文 | 表层模式重复；机械省略清单等不采用；无直接复制 |
| VincentOld/stop-slop-zh | 主入口全文 | 表层清单重复；词频阈值、评分与虚构细节示例不采用 |
| hylarucoder/ai-flavor-remover | 仓库文件、README线索、许可检查 | 未发现根许可证；不复制规则，等待权利说明 |
| OUBIGFA/De-AI-Prompt-Enhancer-Writer-Booster-SKILL | 两份主入口结构及许可检查 | 未发现根许可证；不把可访问当授权，优先采用其已识别的原始许可来源 |
| yiancode/noai-flavor | 结构及完整许可文本 | 代码MIT/内容CC BY 4.0，不误记全MIT；暂无选定的独有内容进入运行包 |
| allenloves/de-ai-tone | 主入口前段及许可 | 台湾繁体措辞及硬阈值不适配；CC BY-SA 4.0可商用但须遵守相应条件，本版未复制 |
| stephenlzc/humanize-mba-text-skill | 主入口前段、目录与规则文件线索 | MBA论文章节约束不用于通用文章；未运行其脚本，无直接采用 |
| redbaronyyyyy-eng/humanizer-zh-academic | 主入口前段及结构 | 学术场景阈值、比例与自报效果未转成通用规则；无直接采用 |

上表未采用不是断言项目无价值；是本次用途、增量、许可证及已阅范围下的决定。原快照与SHA-256保留于工作区研究目录，后续可按新需求继续读，不在运行时自动下载。

## 搜索覆盖与未覆盖

GitHub仓库检索共7组关键词、625条返回、去重482条线索，下载20个候选的固定提交ZIP。多个查询只取首批100条；未遍历所有分页、所有fork、代码搜索或其他平台。因此不是“GitHub全部中文去AI技能”，也不是482个项目都完成了源码审计。

ZIP清单、提交及哈希见工作区 research/upstream-integration-20261003/download-manifest.json；搜索原始清单同目录 search-inventory.json。研究目录不随运行包分发，也不是运行依赖。

旧版0.5.1完整归档于研究目录 legacy-0.5.1-standalone-6。旧natural-writing、paragraph-editing、legal-writing、commentary-negative-checklist已退出运行目录；历史实验只记事实，不再充当写作指令来源。
