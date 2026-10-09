# 铸言文章skill

`zhuyan-article` 是面向已有中文文章的编辑 Skill，用于去除模板化表达、润色、重写和审稿，覆盖法律知识、实务、科技商业与评论。它强调保留事实、作者立场、专业限定和论证关系。

## 当前版本

- 版本：`1.0.0`
- 修订：`release-1`
- 状态：首个正式发布版

本项目把“朱雀人工特征不低于80%、疑似AI不高于20%、AI特征为0”作为持续外部验收目标，但当前版本尚未达到跨题材稳定验收，不能保证任何检测分数，也不能据检测结果判断文章作者身份。正式版表示结构、来源和分发材料完整，不表示检测目标已经实现。

## 仓库结构

实际 Skill 位于 [`zhuyan-article/`](zhuyan-article/)：

- `SKILL.md`：入口、使用示例和工作流程
- `agents/openai.yaml`：界面名称、简介与默认提示语
- `references/`：保真、编辑模式、语体、验收及来源说明
- `licenses/`：采用的第三方 MIT 许可全文
- `THIRD_PARTY_NOTICES.md`：第三方来源、固定提交和采用范围
- `COPYRIGHT.md`：自有内容的版权与使用范围

## 安装和使用

发布到 GitHub 后，安装时应选择仓库中的 `zhuyan-article/` 子目录。手动安装可将该目录完整复制到 Codex Skills 目录，并保留目录名 `zhuyan-article`。

示例：

> 请用铸言文章skill优化下面的公众号文章。允许调整句段顺序，保留全部独立观点、事实和论据，不缩成摘要。只给完整正文。原文如下：……

更多调用示例见 [`zhuyan-article/SKILL.md`](zhuyan-article/SKILL.md)。

## 许可和版权

本仓库不是以单一 MIT 许可覆盖全部内容。崔凯律师享有权利的原创内容与整合编排适用 [`zhuyan-article/COPYRIGHT.md`](zhuyan-article/COPYRIGHT.md)；第三方内容继续适用 [`zhuyan-article/THIRD_PARTY_NOTICES.md`](zhuyan-article/THIRD_PARTY_NOTICES.md) 和 `zhuyan-article/licenses/` 中列明的原许可。

崔凯律师版权所有，禁止蒸馏复制，限个人和小微企业使用。该声明不覆盖第三方开源内容或用户提供的材料。

## 重要边界

- 本 Skill 是文章编辑工具，不替代法律、医疗、财务等专业意见。
- 本地结构校验通过，只证明文件格式和基础引用可用，不证明写作效果或检测成绩。
- 外部检测结果及失败记录保留在 Skill 的实验说明中，不以成功个案宣传稳定效果。
