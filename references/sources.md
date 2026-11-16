# 依据与说明（6 个链接已于 2026-11-16 抽查，均可打开；下列声明已按页面原文校正，使用前仍请自行点开确认）

**官方文档：**
- 积分机制（与模型定价和任务复杂度两个因素有关、循环退费、扣减顺序、有效期；页面没有乘法公式）：workbuddy.cn/docs/workbuddy/Credits
- 积分明细入口（官网个人中心 > 套餐与用量）：workbuddy.cn/docs/workbuddy/Usage
- 模型倍率（最低 Deepseek-V4-Flash x0.06，最高 Kimi-K3 x1.62；页面没有「选性价比模型/不确定用 Auto」的建议，那是作者经验）：workbuddy.cn/docs/workbuddymini/features/Select-Model
- 成本管理（/cost、/context、/clear、模型场景、MCP 开销、子代理隔离、精确提示、计划模式、后台消耗）：workbuddy.cn/docs/cli/costs（CodeBuddy Code 命令行；原则同样适用）
- 钩子系统：workbuddy.cn/docs/cli/hooks
- 子代理模型解析优先级（页面原文从高到低：环境变量 CODEBUDDY_CODE_SUBAGENT_MODEL、入参、项目、全局、内置如 Explore=轻量、主模型）：workbuddy.cn/docs/cli/sub-agents

**环境行为（未在公开文档找到依据，来自作者实测，引用时注明「环境行为」）：** 用户级记忆每次会话注入；工作区记忆为追加日志；定时任务功能；消耗明细页签；轻量子代理与主会话计费模型相同（【环境实测】2026-11-16，单一环境）。以你自己的界面为准。

**【官方规则】终止请求：** 循环执行确认时选「终止请求」会进入退费评估，已产生未出答案的模型消耗可能退回；手动取消不退（来自上面积分机制页面）。本技能不承诺退费。
