# sbx-so

自用补丁二进制镜像仓库，供 PaaS / 免费容器平台部署代理服务使用，避免依赖第三方镜像源。

## 文件列表

| 文件 | 说明 |
|------|------|
| `web` | Xray-core（VLESS / VMess / Trojan / Hysteria2 / Reality） |
| `bot` | Cloudflared（Argo 隧道） |
| `sb` / `sbx.so` | sing-box |
| `v1` | 哪吒监控 agent（v1） |
| `bot.so` / `v1.so` | 对应二进制的 `.so` 后缀变体 |
| `sbsh` | 辅助工具 |

目录结构按架构区分：`amd64/`、`arm64/`。

## 下载地址

```
https://raw.githubusercontent.com/cyoxyu/sbx-so/main/amd64/web
https://raw.githubusercontent.com/cyoxyu/sbx-so/main/amd64/bot
https://raw.githubusercontent.com/cyoxyu/sbx-so/main/arm64/web
https://raw.githubusercontent.com/cyoxyu/sbx-so/main/arm64/bot
```

示例：

```bash
curl -fsSL -o web https://raw.githubusercontent.com/cyoxyu/sbx-so/main/amd64/web && chmod +x web
```
