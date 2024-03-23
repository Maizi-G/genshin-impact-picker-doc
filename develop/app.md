# 构建应用程序

## 本地构建
### Electron

通过在[前端开发](frontend.md#构建)的构建页面步骤中生成静态文件

然后将生成的静态文件 `.vercel/output/static` 手动拷贝到 `electron-static/static` 目录中，并覆盖原有文件。

最后进入 `electron-static` 目录执行：

```bash
$ npm install
$ npm run build # 生成当前系统的可执行文件
$ npm run build-win # 生成 Windows x64 的可执行文件
```

> 如果在执行`npm install`时出现了electron相关的错误，可参考[这篇文章](https://www.bilibili.com/read/mobile?id=4789160)的方法来手动进行安装electron

### Tauri

**需要安装Rust**

在 `Genshin-Impact-Wish-Simulator` 目录下执行：

```bash
$ npm run tauri build
```

## 通过Github Action自动构建

