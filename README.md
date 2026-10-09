# Pkmlife

这是 [pokeman](https://github.com/pokemanok) 的 GitHub Pages 个人主页。站点是纯静态页面（`index.html`），放在仓库根目录，不需要构建。

线上地址：<https://pokemanok.github.io/Pkmlife/>

## 修改内容

直接编辑根目录的 `index.html`：

- 名字现在是占位文字 `pokeman`
- 「关于我」和页首简介都是占位文案
- 「链接」里目前只有 GitHub：<https://github.com/pokemanok>
- 「联系」同样是占位，可改成邮箱或其他方式

改完后提交到 `main` 分支即可。GitHub Pages 会从该分支的根目录重新发布。

## 本地预览

用浏览器直接打开 `index.html`，或在仓库根目录运行：

```bash
python3 -m http.server 8080
```

然后访问 <http://localhost:8080>。

## 开启 GitHub Pages

发布方式：**Deploy from a branch**，分支 `main`，文件夹 `/`（root）。

如果仓库设置里还没有打开 Pages，按下面步骤操作：

1. 打开仓库的 **Settings → Pages**。
2. **Build and deployment** 里，Source 选择 **Deploy from a branch**。
3. Branch 选择 `main`，文件夹选择 `/ (root)`。
4. 保存后等待一两分钟，再访问 <https://pokemanok.github.io/Pkmlife/>。

说明：免费账号的 GitHub Pages 只对公开仓库提供。如果这个仓库是私有的，需要先将仓库设为 Public，或使用支持私有 Pages 的方案，站点才会对外可访问。
