# 构建应用程序

## 本地构建
### Electron

通过在[前端开发](frontend.md#构建)的构建步骤中生成静态文件

然后将生成的静态文件 `.vercel/output/static` 手动拷贝到 `electron-static/static` 目录中，并覆盖原有文件。

最后进入 `electron-static` 目录执行：

```bash
$ npm install
$ npm run build # 生成当前系统的可执行文件
$ npm run build-win # 生成 Windows x64 的可执行文件
```

> 如果在执行`npm install`时出现了electron相关的错误，可参考[这篇文章](https://www.bilibili.com/read/mobile?id=4789160)的方法来手动进行安装electron

### Tauri

>在这之前，请按Tauri的[文档](https://tauri.app/v1/guides/getting-started/prerequisites)配置好相应软件，并确保在[前端开发](frontend.md#安装依赖)中已经安装好项目依赖


在 `Genshin-Impact-Wish-Simulator` 目录下执行：

```bash
$ npm run tauri build
```

## 通过Github Action自动构建

如果因为一些原因而无法进行构建程序，可以通过CI的方式来进行构建

CI配置文件在`.github/workflows`目录下

