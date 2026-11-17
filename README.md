# workbuddy-credit-saver

WorkBuddy 积分用得太快？这是一个 WorkBuddy 技能：先问清需求、选对模型和档位、长会话快速交接、脚本优先、及时停止空转。

WorkBuddy credits burning too fast? A WorkBuddy skill: clarify requirements first, route models, hand off long sessions, scripts before agents, kill idle tasks. Adapted from [claude-usage-limit-fix](https://github.com/superlady2049-source/claude-usage-limit-fix) (for Claude Code).

## 安装

方式一（本地 ZIP）：下载本仓库 ZIP，在 WorkBuddy 技能管理里选「本地 ZIP」导入。

方式二（放进技能目录）：

```bash
git clone https://github.com/superlady2049-source/workbuddy-credit-saver ~/.workbuddy/skills/workbuddy-credit-saver
```

目录位置以你的 WorkBuddy 版本为准；导入后在新对话里说「我的积分用得太快了，怎么办？」，看它是否引用本技能。

## 说明

- 核心在 `SKILL.md`，细则在 `references/`，模板在 `templates/`，需要时才读。
- 官方依据与「环境实测」说明见 `references/sources.md`；积分数字和功能以你的界面和官方文档为准，效果没有对照实验。
- Claude Code 用户请用 claude-usage-limit-fix。

## 版本历史

- v1.0.0：初版。
- v1.1.0：新增触发/不触发条件、4 行默认输出、异常与降级表、证据分级、FAQ、示例、模板；核心瘦身。
- v1.2.1：取消子代理用量硬停线，改为「提醒线只告知、确认线先交方案」；新增「评审少走弯路」四条（先写评分表、真实数据复核、规则冲突即 bug、检查脚本防误判）。
- v1.2.0：七类浪费表重排为八类，新增「怎么发现」列和第八类「经验没用起来」；精简每轮常驻的 SKILL.md 正文，会话卫生与实测数字、选模型、异常与降级挪到 references/；新增 overview.md。

效果尚未被证明，初步实测见 SKILL.md。

## 作者

**KAI LI** · AI经营改善顾问 · AI Operations Improvement Consultant

邮箱：superlady2049@gmail.com

扫码添加飞书联系人：

<img src="assets/lark-qr.png" width="220" alt="KAI LI 飞书二维码">

扫码添加企业微信：

<img src="assets/wecom-qr.png" width="220" alt="KAI LI 企业微信二维码">

MIT License
