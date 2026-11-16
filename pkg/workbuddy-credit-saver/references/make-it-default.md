# 让技能默认生效（技能是软触发，不保证每次都用）

- **WorkBuddy 桌面 App：** 没有钩子配置入口。硬约束渠道是用户级记忆文件（每次会话自动注入）：加一条强制规则「派子代理、选模型、开长任务、批量生成前，先调用 workbuddy-credit-saver 技能」。
- **CodeBuddy Code 命令行：** 完整支持钩子，配置在 `~/.codebuddy/settings.json` 的 hooks，可用 PreToolUse（派活闸门：不写 model 拦截、推理档没写【理由】拦截）、SessionStart（会话开始注入省积分提醒）等。可移植原仓库 claude-usage-limit-fix 的钩子脚本，matcher 写 `^Agent$`。
- 同一类浪费出现第二次，必须升级成强制规则（App）或钩子（命令行），不能只写在技能里。
