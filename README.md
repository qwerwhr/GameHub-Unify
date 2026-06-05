# GameHub-Unify
GameHub-Unify 全平台PC游戏聚合管理器

功能特性
🎮 多平台客户端管理 - Steam/Epic/GOG/Ubisoft/EA/Rockstar 统一管理
👤 账号一键登录 - AES-GCM加密存储，本地安全存储
🎁 喜加一自动领取 - 一键批量领取全平台免费游戏
🚀 双模式加速器 - 内嵌内核 + 外置客户端
⏱️ 精准计时计费 - 游戏退出即时停止扣时长
🔧 运行环境修复 - VC++/DirectX/.NET 一键安装
🎯 修改器资源库 - 风灵月影等正版跳转下载
💰 全平台比价 - 实时价格 + 历史史低
技术栈
语言: Rust 2021 Edition
GUI: eframe/egui
异步: tokio
数据库: SQLite
加密: AES-GCM
项目结构
gamehub-unify/
├── Cargo.toml
├── config/                    # 配置文件
│   ├── app.toml
│   ├── platform_cfg.json
│   └── accel_cfg.json
├── src/
│   ├── main.rs               # 程序入口
│   ├── core/                 # 核心业务层
│   ├── platform_core/        # 平台抽象层
│   ├── platform_adapter/     # 平台具体实现
│   ├── accelerator_core/     # 加速器抽象层
│   ├── accelerator_adapter/  # 加速器具体实现
│   ├── tool_center/          # 工具中心
│   ├── spider/               # 爬虫模块
│   ├── cache/                # 三级缓存
│   ├── db/                   # 数据库
│   ├── ui/                   # GUI页面
│   ├── utils/                # 工具函数
│   └── error/                # 错误处理
├── assets/                   # 静态资源
└── tests/                    # 测试
快速开始
编译
cargo build --release
运行 GUI
cargo run --features gui
运行 CLI
cargo run --features cli -- --help

目前处于立项中<br><br>
