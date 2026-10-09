# Pkmlife

[pokeman](https://github.com/pokemanok)（破壳漫）的 GitHub Pages 个人主页。纯静态，无构建步骤。

- 站点：<https://pkm.life> · <https://pokemanok.github.io/Pkmlife/>
- 加密聊天演示：<https://pkm.life/chat/> · <https://pokemanok.github.io/Pkmlife/chat/>

## 内容

- `index.html` — 中文个人主页与 **GBA 汉化作品**（木乃伊归来、终结者3、环游世界80天）
- `chat/` — 浏览器端 AES-GCM 加密聊天演示（口令派生密钥；BroadcastChannel + localStorage；可导出/粘贴密文跨设备）

## 加密聊天说明

1. 双方约定同一口令与房间名，在 `/chat/` 进入。
2. 明文只在本地加密前后短暂存在；写入存储与跨标签同步的是密文 JSON。
3. **不会**把明文或口令放进 URL / query。
4. 与助手对话：把密文 JSON 粘贴给助手，助手用同一口令解密后回复密文；或双方配置同一共享口令。
5. GitHub Pages 无后端：跨设备请交换密文，或自行接 WebSocket/WebRTC（只传密文）。

## 本地预览

```bash
python3 -m http.server 8080
```

打开 <http://localhost:8080> 与 <http://localhost:8080/chat/>。

## Pages

Source：**Deploy from a branch**，分支 `main`，目录 `/`（root）。自定义域见 `CNAME`（`pkm.life`）。
