---
description: 本文主要教学用户如何部署本点名器
---

# 部署教程

## 本地使用(推荐)

### 通过Release获取应用程序

从[github release](https://github.com/cyanial/genshin-impact-picker/release/latest)中按照使用提示来获取对应系统的程序包

> Tips:zip的文件需要**完整解压**后才可以运行

### 通过Action(CI构建)获取应用程序

**需要登录Github账号**

相对于Release，CI版本可提前体验尚未正式发布的更新内容(可能不稳定)

从[Github Action(CI)](https://github.com/cyanial/genshin-impact-picker/actions/workflows/app.yml)中获取对应系统的程序包

## 在线使用

> Tips:因为在线部署后可能存在网络波动等问题，没有本地流畅，因此不推荐使用本方法

### 公共站点todo



### Netlify 一键部署

通过下方按钮可直接一键部署至 Netlify（本仓库已内置配置文件，适合懒人使用）。

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/cyanial/genshin-impact-picker&base=Genshin-Impact-Wish-Simulator)

### Vercel 一键部署

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/cyanial/genshin-impact-picker)

部署成功后，进入 `Settings-General`，将 `Build & Development Settings` 下的 `Root Directory` 设置为 `Genshin-Impact-Wish-Simulator`。回到 `Deployments` 页面，点击当前部署右侧的三个点，选择 `Redeploy`。等待部署完成后，访问 Vercel 提供的域名即可。