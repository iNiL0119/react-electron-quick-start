### React与Electron项目创建

1. 创建React项目：npx create-react-app react-electron-quick-start
2. 进入项目：cd react-electron-quick-start
3. 运行React项目：yarn start / yarn run start（个人习惯用后者）
4. 安装electron包：yarn add electron --dev
5. 新建Electron入口文件main.js，内容与electron-quick-start中的main.js内容相同，只是需要将窗口加载地址修改为项目url地址（mainWindow.loadFile('index.html') -> mainWindow.loadURL('http://localhost:3000/')
6. 修改package.json文件，新增"main": "main.js", "homepage": ".", "scripts"中新增"electron": "electron ."
6. 运行yarn run start
7. 运行yarn run electron