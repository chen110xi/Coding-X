#### Coding-Cli

$ ssh username@cli.coding.net  (username 为你的 Coding 个性后缀)
```

               _ _                        _ _
  ___ ___   __| (_)_ __   __ _        ___| (_)
 / __/ _ \ / _` | | '_ \ / _` |_____ / __| | |
| (_| (_) | (_| | | | | | (_| |_____| (__| | |
 \___\___/ \__,_|_|_| |_|\__, |      \___|_|_|
                         |___/
Welcome to coding-cli.

tvvocold $ help
NAME:
   coding - coding.net command line tool

USAGE:
   command [subcommand] [command options] [arguments...]

VERSION:
   0.1.1

COMMANDS:
    me		账户信息
    avatar	查看用户头像
    help	help
    project	项目相关操作
    task	任务相关操作
    mr		MR 相关操作
    pp		冒泡相关操作

GLOBAL OPTIONS:
   --version, -v	print the version
```

#### 命令行创建 Merge Request

- push 到 mr/master/branch_name 分支即可自动创建 MR，如 $git push origin Feature-x:mr/master/Feature-X
- 自动创建的使用最后一个 commit message 作为标题和内容
- 自动解析 commit message 中 @ 的人，自动加成评审者，自动# 加为关联资源
- 自动创建出来的新的分支，只能有创建者再次 push 到这个分支，也允许 force push





