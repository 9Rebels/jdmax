## JDMAX

#### 声明: 此库所有内容仅用于测试学习，测试完后请自行删除！！！
#### 声明: 此库所有内容仅用于测试学习，测试完后请自行删除！！！
#### 声明: 此库所有内容仅用于测试学习，测试完后请自行删除！！！

#### 青龙拉取代码：

```
rm -rf /ql/repo/9Rebels_jdmax && ql repo https://github.com/9Rebels/jdmax.git "jd_|ql_|jx_" "activity|backUp" "^jd[^_]|ql|utils|sendNotify"

```

#### Arcadia 面板拉库（[项目地址](https://arcadia.cool)）
```
arcadia repo jdmax "https://github.com/9Rebels/jdmax.git" main --updateTaskList true --whiteList "^jd_|^jx_" --blackList "^jd_(CheckCK)"
```

定时随意，不要设置为每秒或每分钟

## 注意

默认自带定时，如发现定时为 ‘1 1 1 1 \*’ 类似，表示 手动运行。

## 简要流程

### 旧版本青龙执行：1.2.4.5.6 条

1、部署青龙并登陆。

2、到配置管理 config.sh 修改，差不多在 17 行（特别注意，没有修改此配置，sh 类型任务拉不下来）；

RepoFileExtensions="js py"修改为 RepoFileExtensions="js py sh" 保存；

3、到订阅管理创建订阅并运行；

4、订阅运行完毕，到定时任务搜索依赖安装任务执行；

5、到环境变量，创建变量，名称: JD_COOKIE,值：获取的数据，多个依次创建；

6、配置通知，通知的 key 填写到配置管理 config.sh 文件；

7、sendnotify.js 文件请拷贝库里的到青龙 deps 目录下，否则会自带覆盖；

## 相关说明

1、[相关说明](https://github.com/9Rebels/jdmax/wiki)

