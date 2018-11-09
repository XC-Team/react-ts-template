# react-ts-template

>Zenquan的react-ts-cli项目脚手架模板文件

## Document

- [前端](./App/readme.md)
- [后端](./Server/readme.md)

## App

>基于[WLM-TypeScript-React-Starter](https://github.com/welearnmore/WLM-TypeScript-React-Starter)搭的react-typescript脚手架,方便日后写此类项目。集成了 [ React + React-Router + Redux + Redux-Thunk ]，旨在为 Web 应用程序开发者提供 “开箱即用” 的 TypeScript 工程，开发者只需下载此项目，根据范例即可编写复杂大型的 React 应用。 

### 编译环境：

- node.js > 8.0
- typescript > 3
- git
- yarn
- 支持 editorconfig
- 支持 tslint
- 支持 css modules

### Install

```bash
$ git clone https://github.com/Zenquan/react-ts-template.git
$ cd App
$ yarn
or
$ npm start
```

直接使用浏览器访问本地文件 `index.html`，即可。（更多命令可查看 package.json 的 scripts 字段）

### 目录结构

顶级目录结构如下：

- src 项目源文件
- typings 自定义声明
- dist 编译后的目录

`src` 目录结构如下：

- components # 通用组件
- pages #页面
  - Home # 自定义的目录
    - flow # redux 相关
      |- actions
      |- reducers
      |- constants
    - components # 此页面组件
    - index.tsx # 页面
    - style.css # 样式
    - types.d.ts # ts 声明
- global # redux store 配置 以及 global reducers
- index.tsx # 入口
- app.tsx # layout & routes

### 使用

在 `pages` 中创建一个目录，假设名为 `Home` （这是开发者可自己约定的命名），然后创建 `index.tsx`，`style.less`文件和 `flow` 目录（创建 `actions.ts`，`constants.ts`，`mainPageReducers.ts`），【如果你不使用redux，完全可以不创建 `flow` 目录】。

## Server
