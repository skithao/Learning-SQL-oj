# Sunsky-SQL判题系统

## 概览

SQL判题系统是一个交互式的在线平台，旨在通过各种练习和挑战来增强SQL语言的学习和实践。它使用户能够提交SQL查询，在安全的环境中执行它们，并立即获得关于它们解决方案的反馈。该系统支持多种题型，包括填空题和基于实际场景的问题。

## 核心功能

- **用户认证**：安全的 用户注册、登录和权限管理，以确保数据安全和隔离。
- **题目管理**：创建、存储、编辑和删除题目，包括题目类型（填空题、实践题）和内容。
- **练习和答题**：用户可以在线练习SQL语句，提交答案，并接收反馈。
- **题目提交**：用户可以提交新的SQL题目，包括题目名称、描述、示例代码和评分要求。
- **评分引擎**：核心功能，用于解析和执行SQL语句，并根据题目要求验证结果。
- **前端界面**：用户友好的界面，用于展示题目、答题和提交新题目。
- **数据库设计**：设计数据库模型以存储用户信息、题目信息和题目结果。
- **安全性**：确保SQL执行环境的安全，防止SQL注入和其他安全威胁。
- **反馈机制**：提供详细的反馈，帮助用户理解错误并改进。

## 技术栈

- **后端**：使用Flask框架的Python进行API开发。
- **ORM**：SQLAlchemy用于数据库交互和动态模型生成。
- **前端**：HTML、CSS、JavaScript，并可选React或Vue.js来构建动态用户界面。
- **SQL编辑器**：Ace Editor提供丰富的SQL编码体验。
- **认证**：Flask-Login用于处理用户会话。
- **表单处理**：Flask-WTF用于表单验证和处理。
- **管理界面**：Flask-Admin用于数据库CRUD操作。
- **安全性**：Flask-Sandbox用于安全执行SQL语句。
- **异步任务**：Celery用于处理后台任务（可选）。
- **数据库**：PostgreSQL、MySQL或SQLite。
- **部署**：Docker用于容器化，确保环境一致性。

## 目录结构

```plaintext
sql-judge-system/
│
├── api/                 # API接口文件
│   ├── __init__.py
│   ├── routes.py        # 路由定义
│   └── models.py        # 数据模型定义
│
├── core/                 # 核心逻辑文件
│   ├── __init__.py
│   ├── executor.py      # SQL语句执行器
│   ├── parser.py        # SQL语句解析器
│   └── comparator.py    # 结果比较器
│
├── utils/                # 工具文件
│   ├── __init__.py
│   ├── database.py      # 数据库连接工具
│   └── security.py      # 安全工具
│
├── templates/            # 前端模板文件（如果使用）
│   ├── index.html
│   └── ...
│
├── static/               # 前端静态文件（如果使用）
│   ├── css/
│   ├── js/
│   └── ...
│
├── config/               # 配置文件
│   ├── config.py        # 配置类
│   └── secrets.py       # 敏感信息配置
│
├── main.py                # 项目入口文件
├── requirements.txt      # Python依赖包
└── README.md             # 项目文档
```git clone https://github.com/Linzecong/LPOJ.git。
3. **运行系统**：使用`python main.py`运行Flask应用程序。
4. **访问界面**：在指定的主机和端口通过浏览器访问用户界面。

## 贡献

有关贡献指南和如何设置开发环境的详细信息，请参考[贡献指南](https://github.com/your-username/sql-judge-system/blob/main/CONTRIBUTING.md)。

## 许可证

SQL判题系统是开源软件，根据[MIT许可证](https://opensource.org/licenses/MIT)授权。
