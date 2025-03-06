# Eliza

## （可选）调整默认角色文件

Open `agent/src/character.ts` to modify the default character. Uncomment and edit.

### 启动角色（已经模仿好的角色是DePIN_News.json）

To load custom characters instead:
- Use `pnpm start --characters="path/to/your/character.json"`
- Multiple character files can be loaded simultaneously

### 添加客户端

```diff
- clients: [],
+ clients: ["twitter", "discord"],
```

## 复制 .env.example 

```bash
cp .env.example .env
```

\* Fill out the .env file with your own values.

### 在 .env文件中添加登录信息

```diff
-DISCORD_APPLICATION_ID=
-DISCORD_API_TOKEN= # Bot token
+DISCORD_APPLICATION_ID="000000772361146438"
+DISCORD_API_TOKEN="OTk1MTU1NzcyMzYxMT000000.000000.00000000000000000000000000000000"
...
-OPENROUTER_API_KEY=
+OPENROUTER_API_KEY="sk-xx-xx-xxx"
...
-TWITTER_USERNAME= # Account username
-TWITTER_PASSWORD= # Account password
-TWITTER_EMAIL= # Account email
+TWITTER_USERNAME="username"
+TWITTER_PASSWORD="password"
+TWITTER_EMAIL="your@email.com"
```

## 绑定依赖并启动

```bash
pnpm i && pnpm start
```
