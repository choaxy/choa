# cyoxyu

自用补丁二进制镜像仓库，供 PaaS / 免费容器平台部署代理服务使用，避免依赖第三方镜像源。
`Plugins/` 目录另存官方插件原版镜像，供各替换器在官方源不可达时兜底下载。

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
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/amd64/web
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/amd64/bot
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/arm64/web
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/arm64/bot
```

示例：

```bash
curl -fsSL -o web https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/amd64/web && chmod +x web
```

## Plugins（官方插件镜像）

官方插件原版包，替换器优先走官方源，此处为兜底镜像。均已校验大小与 SHA-256。

| 文件 | 官方来源 | 大小 | SHA-256 |
|------|----------|------|---------|
| `EssentialsX-2.21.1.jar` | [EssentialsX/Essentials Release 2.21.1](https://github.com/EssentialsX/Essentials/releases/download/2.21.1/EssentialsX-2.21.1.jar) | 4,655,797 | `15dd7f8713e613a1ddeada792db660a88c8bf69015bc13f1a9f9e37f6d44cf5a` |
| `Geyser-Spigot.jar` | [Modrinth Geyser (cEESv2Kx)](https://cdn.modrinth.com/data/wKkoqHrH/versions/cEESv2Kx/Geyser-Spigot.jar) | 19,662,581 | `b754bb257976549553239be82c4b1a8ca97bac997c8799fdee5a28a287e7fda6` |
| `lithium-fabric-0.21.4+mc1.21.11.jar` | [Modrinth Lithium (Ow7wA0kG)](https://cdn.modrinth.com/data/gvQqBUqZ/versions/Ow7wA0kG/lithium-fabric-0.21.4%2Bmc1.21.11.jar) | 900,462 | `5135c41da5b43cbdcb29424bde65195143ac4084e23834c8eac065942201c78b` |

镜像下载地址：

```
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/Plugins/EssentialsX-2.21.1.jar
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/Plugins/Geyser-Spigot.jar
https://raw.githubusercontent.com/cyoxyu/cyoxyu/main/Plugins/lithium-fabric-0.21.4%2Bmc1.21.11.jar
```
