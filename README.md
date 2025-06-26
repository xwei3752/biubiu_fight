# Biubiu Fight - 像素风格格斗游戏

一个使用Phaser.js开发的像素风格格斗游戏，支持双人对战。

## 功能特性

- 🎮 像素风格的游戏画面
- ⚔️ 丰富的战斗系统
  - 近战攻击（鼠标左键/J）
  - 远程攻击（鼠标右键/K）
  - 防御系统（A键）
- 🏃‍♂️ 流畅的移动控制
  - Space键：跳跃
  - A键：后退/防御
  - D键：前进
- 🌐 多人对战支持
  - 使用Multisynq实现实时同步
  - 支持多个玩家同时游戏

## 安装和运行

1. 安装依赖：
```bash
npm install
```

2. 启动开发服务器：
```bash
npm run dev
```

3. 在浏览器中打开 `http://localhost:3000`

## 游戏控制

- **Space** - 跳跃
- **A** - 后退/防御
- **D** - 前进
- **鼠标左键** - 近战攻击
- **鼠标右键** - 远程攻击

## 技术栈

- **Phaser.js** - 游戏引擎
- **Vite** - 构建工具
- **Multisynq** - 多人对战同步

## 项目结构

```
src/
├── main.js                 # 游戏入口
├── scenes/                 # 游戏场景
│   ├── MenuScene.js       # 菜单场景
│   └── GameScene.js       # 游戏主场景
├── entities/              # 游戏实体
│   └── Player.js          # 玩家类
└── utils/                 # 工具类
    ├── PixelFontGenerator.js    # 像素字体生成器
    └── MultiplayerSimulator.js  # 多人对战模拟器
```

## 开发说明

游戏使用Phaser.js的物理引擎实现碰撞检测和重力效果。玩家角色具有完整的生命值系统、攻击冷却和防御机制。

多人对战功能通过Multisynq实现实时数据同步，包括：
- 玩家位置同步
- 攻击动作同步
- 生命值同步
- 玩家加入/离开事件

## 构建生产版本

```bash
npm run build
```

构建后的文件将输出到 `dist` 目录。

## 许可证

MIT License 