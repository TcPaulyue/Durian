## 项目结构文档树
```
## 项目结构文档树
Durian
.
├── config      配置文件，主要用于配置邮箱信息、result路径下结果文件最大个数
├── .gitignore  git版本控制忽略的文件
├── docs        项目文档
│   ├── config.md       配置规则文档
│   ├── develop.md      开发文档
│   ├── readme.txt      使用指南
│   ├── rule.txt        规则文件说明
│   ├── cron.txt        linux定时任务配置
│   └── tree.md         文档树
├── durian.py       程序入口
├── logs            日志文件
│   └── codechecktool.log
├── README.md       README
├── result          扫描结果，文件内文件个数可以在config中配置
│   ├── result.json
│   ├── s77345grk5mh
│   └── s77345tc2fjf
├── rules               扫描规则
│   ├── CVI-100001.xml
│   ├── CVI-100002.xml
│   ├── CVI-100003.xml
│   ├── CVI-100004.xml
│   ├── CVI-100005.xml
│   ├── CVI-110001.xml
│   ├── CVI-110002.xml
│   ├── CVI-120001.xml
│   ├── CVI-200001.xml
│   ├── languages.xml       语言
│   └── vulnerabilities.xml     缺陷类型
├── src             源码
│   ├── clangtool.py      libclang对AST的操作
│   ├── cli.py            cli扫描模式
│   ├── config.py         配置
│   ├── engine.py         后续api模式可以将方法抽象到engine
│   ├── __init__.py       解析参数，调用cli
│   ├── log.py            日志打印
│   ├── __pycache__
│   │   ├── cli.cpython-36.pyc
│   │   ├── __init__.cpython-36.pyc
│   │   ├── log.cpython-36.pyc
│   │   ├── send_mail.cpython-36.pyc
│   │   └── __version__.cpython-36.pyc
│   ├── rule.py             规则扫描操作
│   ├── send_mail.py        发送邮件
│   ├── util.py             工具类
│   ├── __version__.py      版本信息
└── test            测试
    ├── test_clang      libclang AST测试
    │   ├── AnalysisAST.py
    │   ├── asttree.py
    │   ├── get_func_detail.py
    │   ├── get_type.py
    │   ├── get_vars.py
    │   └── person.cpp
    ├── test_eamil.py
    ├── test_mulpro.py
    ├── test_re.py
    └── test_util.py
```

