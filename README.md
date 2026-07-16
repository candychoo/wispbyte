Wispbyte 自动登录机器人
每 3 天自动登录 wispbyte 服务器，防止掉线。

配置步骤
创建 Telegram Bot  创建 Telegram 机器人

找 @BotFather 创建 Bot
获取 TG_BOT_TOKEN
发消息给 Bot，获取 TG_CHAT_ID（可用 @userinfobot）
发消息给 Bot，获取 TG_CHAT_ID （可用 @userinfobot ）
GitHub Secrets 设置  GitHub 秘密设置

进入仓库 → Settings → Secrets and variables → Actions
进入仓库 → 设置 → 秘密和变量 → 操作
添加以下 Secrets：
Name  姓名	Value  价值
TG_BOT_TOKEN	你的 Bot Token  您的机器人令牌
TG_CHAT_ID	你的 Chat ID
LOGIN_ACCOUNTS	email1:pass1,email2:pass2
邮箱1:密码1，邮箱2:密码2
启用 Actions  启用操作

第一次运行会自动安装 Chromium 并执行
定时规则
cron: '0 20 */2 * *'  # 每两天 UTC 20:00（北京 4:00）
