# {{name}}

> {{description}} > {{createDate}}

## 项目依赖安装

```bash
$ yarn
# or
$ npm i
```

你也可以安装 nrm 管理 npm 镜像源，安装命令：

```bash
$ npm i -g nrm
$ nrm ls
$ * npm ---- https://registry.npmjs.org/		# 带星号的是你现在所使用的镜像源
  cnpm --- http://r.cnpmjs.org/
  taobao - https://registry.npm.taobao.org/
  nj ----- https://registry.nodejitsu.com/
  rednpm - http://registry.mirror.cqupt.edu.cn/
  npmMirror  https://skimdb.npmjs.com/registry/
  edunpm - http://registry.enpmjs.org/
$ nrm use cnpm
```

### 运行开发环境

```bash
$ yarn dev
# or
$ npm run dev
```

### 生产环境构建

```bash
$ yarn build
```

### 运行测试用例

```bash
$ yarn test
# or
$ npm run test
```

### 项目目录

```bash
.
├── README.md
├── babel.config.js				# babel配置，用于将ES6+
├── jest.config.js
├── node_modules/					# 存放依赖包管理，不允许提交到服务器
├── package.json
├── postcss.config.js
├── yarn.lock
├── tests/								# 测试用例
├── public
│   ├── favicon.ico
│   └── index.html				# SPA的HTML模板
├── dist/									# 构建之后的目录，一般不需要理会
├── src										# 开发目录
│   ├── App.vue						# 最高级组件，只被main.js引用
│   ├── assets						# 放置静态资源，如图片、样式等
│   ├── components				# 放置公用组件
│   ├── main.js						# 根文件，打包入口
│   ├── router.js					# 路由配置
│   ├── store.js					# Vuex全局状态管理
└── └── views							# 视图组件，一般用于处理交互逻辑
```
