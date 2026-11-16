# CodeBuddy 命令行与钩子（仅命令行用户）

WorkBuddy 桌面端没有钩子入口，见 `make-it-default.md`。以下只适用于 CodeBuddy Code 命令行。

- 命令行完整支持钩子，配置在 `~/.codebuddy/settings.json` 的 hooks，可用 PreToolUse（派活闸门：不写 model 拦截、推理档没写【理由】拦截）、SessionStart（会话开始注入省积分提醒）等。
- 可移植原仓库 claude-usage-limit-fix 的钩子脚本，matcher 写 `^Agent$`。
- 官方成本文档（`/cost`、`/context`、`/clear` 等）与钩子系统页面见 `sources.md`。
- 同一类浪费出现第二次，应升级成钩子，不能只写在技能里。
