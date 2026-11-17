---
name: workbuddy-credit-saver
slug: workbuddy-credit-saver
displayName: WorkBuddy 省积分管家
version: 1.2.0
author: KAI LI
description: WorkBuddy 任务成本控制与会话卫生：派子代理、读大量资料、批量生成、选模型、长会话交接、后台任务等待时使用；先判断要不要澄清、走哪条最省的路径、何时停止或交接。只提供规划建议，不读取账户数据，不自动取消任务、改模型或承诺退费。Plan WorkBuddy task cost and session hygiene.
---

# WorkBuddy 省积分管家

改编自 claude-usage-limit-fix（MIT，作者 KAI LI）。**先问清要什么，再选最便宜够用的路径；不干活的任务立刻停；上下文大了再交接。** 效果尚未被证明，初步实测见 references。

## 30 秒快速使用

1. 「这个任务会不会很费积分？先给我最省的做法。」
2. 「我要读整个资料库，先判断范围再动手。」
3. 「批量做 30 张图，先确认再开跑。」
4. 「这个会话很长了，要不要交接？」

## 触发条件（命中任一条）

派子代理或拆多任务；读整本 PDF/PPT/代码库；批量生成；问用哪个模型；说积分消耗太快；同一交付物改或评审到第 3 轮；会话很长还要继续；有后台任务、轮询、等待授权；问要不要交接。

## 不触发条件

需求明确一两步能完成；用户说「直接做」；只改一句话；与成本无关；先问一轮比直接试一次还贵。

## 默认输出（只要 4 行）

1. 模式与成本等级：低 / 中 / 高 / 未知
2. 缺失的输入
3. 推荐路径
4. 下一步一个最小动作

## 派活前自检

1. 四要素（对象、范围、用途、验收）齐了吗？2. 能不做吗？3. 脚本或已有结果能用吗？4. 真需要子代理吗？5. 档位写明了吗？6. 预计超过提醒线（或确认线）吗？7. 输入是精选材料吗？8. 只写了预估、没写硬停线吗？9. 有残留后台任务吗？10. 批量生成出过样品吗？

细节按需读 references/：`forecast.md`（大用量预测、八类浪费）、`session-and-models.md`（会话卫生、选模型、实测）、`fallbacks.md`（澄清、异常与降级）、`evidence-levels.md`、`examples.md`、`faq.md`、`sources.md`。

## 关于作者

KAI LI，AI 经营改善顾问（AI Operations Improvement Consultant）。邮箱 superlady2049@gmail.com；飞书二维码 `assets/lark-qr.png`，企业微信二维码 `assets/wecom-qr.png`。
