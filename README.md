# GameHub-Unify
GameHub-Unify 全平台PC游戏聚合管理器<br><br>

功能特性<br><br>
🎮 多平台客户端管理 - Steam/Epic/GOG/Ubisoft/EA/Rockstar 统一管理<br><br>
👤 账号一键登录 - AES-GCM加密存储，本地安全存储<br><br>
🎁 喜加一自动领取 - 一键批量领取全平台免费游戏<br><br>
🚀 双模式加速器 - 内嵌内核 + 外置客户端<br><br>
⏱️ 精准计时计费 - 游戏退出即时停止扣时长<br><br>
🔧 运行环境修复 - VC++/DirectX/.NET 一键安装<br><br>
🎯 修改器资源库 - 风灵月影等正版跳转下载<br><br>
💰 全平台比价 - 实时价格 + 历史史低<br><br>
技术栈<br><br>
语言: Rust 2021 Edition<br><br>
GUI: eframe/egui<br><br>
异步: tokio<br><br>
数据库: SQLite<br><br>
加密: AES-GCM<br><br>
项目结构<br><br>
gamehub-unify/<br><br>
├── Cargo.toml<br><br>
├── config/                    # 配置文件<br><br>
│   ├── app.toml<br><br>
│   ├── platform_cfg.json<br><br>
│   └── accel_cfg.json<br><br>
├── src/<br><br>
│   ├── main.rs               # 程序入口<br><br>
│   ├── core/                 # 核心业务层<br><br>
│   ├── platform_core/        # 平台抽象层<br><br>
│   ├── platform_adapter/     # 平台具体实现<br><br>
│   ├── accelerator_core/     # 加速器抽象层<br><br>
│   ├── accelerator_adapter/  # 加速器具体实现<br><br>
│   ├── tool_center/          # 工具中心<br><br>
│   ├── spider/               # 爬虫模块<br><br>
│   ├── cache/                # 三级缓存<br><br>
│   ├── db/                   # 数据库<br><br>
│   ├── ui/                   # GUI页面<br><br>
│   ├── utils/                # 工具函数<br><br>
│   └── error/                # 错误处理<br><br>
├── assets/                   # 静态资源<br><br>
└── tests/                    # 测试<br><br>
快速开始<br><br>
编译<br><br>
cargo build --release<br><br>
运行 GUI<br><br>
cargo run --features gui<br><br>
运行 CLI<br><br>
cargo run --features cli -- --help<br><br>

目前处于立项中<br><br>
