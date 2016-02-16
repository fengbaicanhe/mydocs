# Gradle 命令大全


gradle 命令基本语法

`
gradle [option...] [task...]
`

| 命令                                | 解释                           |
|----------------                     |--------------------------------|
| -?, -h, --help                     | 显示 gradle 命令帮助             |
| -a, --no-rebuild                     | 不重新构建 项目依赖               |
| -b, --build-file                     | 指定构建文件位置                 |
| -c, --settings-file                 | 设置 gradle settings 配置文件    |
| --configure-on-demand               | 只有相关的工程会随着本次构建而构建，对于大型多工程项目来说，这能够更快的编译项目[孵化阶段] |
| --console                             |  指定控制台输出的类型，可选值有 **plain** , **auto**(默认) , **rich**   |
| --continue   | 在一个任务失败后，继续其他 任务的 执行 |
| -D , --sysstem-prop | 设置JVM的系统参数，比如 `-Dmyprop=myvalue` |
| -d,--debug | 启用debug日志模式(包括普通的stacktrace) |
| --daemon  | 使用Gradle的守护进程来运行构建，如果守护进程没有运行，则会启动守护进程|
| --foreground | 在前台启动Gradle守护进程(孵化中) |
| -g, --gradle-user-home | 指定Gradle 的用户主目录 |
| -gui | 启动 Gradle 的 图形化界面 |
| -I, --init-script | 指定一个初始化脚本 |
| -i, --info | 设置日志级别为 `info` |
| -m, --dry-run | 禁用所有的 task action 来执行构建任务 |
| --max-workers | 设置Gradle所有的worker并发数量 |
| --no-color | 不对控制台de输出进行颜色高亮 [此配置项已经**过期**, 使用 `--console=plain` 来替代] |
| --no-daemon | 不使用Gradle的守护进程来运行构建 |
| --offline | 使用离线模式进行构建 |
| -P, --project-prop | 为构建脚本设置项目的属性参数，如 `-Pmyprop=myvalue` |
| -p, --project-dir | 指定Gradle的启动目录，默认为当前目录 |
| --parallel | 并行构建项目，Gradle 会尝试使用线程池最合适的数量[孵化中] |
| --parallel-threads | 并行构建项目，使用指定数量的线程池，[**过期** - 请使用 --parallel，可以选择添加 --max-workers[孵化中] 来设置数量 ] |
| --profile | 记录构建时间，并在 <build_dir>/reports/profile目录下生成一个报告文件 |
| --project-cache-dir | 设置项目级别的缓存文件夹，默认为项目根目录下的.gradle文件夹 | 
| -q, --quiet | 静默模式，只输出错误日志 |
| --recompile-scripts | 强制构建脚本(build.gradle)重新编译 |
| --refresh-dependencies | 刷新依赖的状态 |
| --rerun-tasks | 忽略之前 任务 结果缓存 |
| -S, --full-stacktrace | 为所有异常输出完整的(非常冗长)stacktrace |
| --stop| 如果Gradle的守护进程正在运行，则停止Gradle的守护进程 |
| -t, --continuous | 启用持续构建，Gradle不会退出，并且当task有改变的时候，会重新执行有改变的task | 
| -u， --no-search-upward | 不向上搜索父文件夹的settings.gradle文件 |
| -v, --version | 输出Gradle版本信息 |
| -x, --exclude-task | 指定一个task，这个task在执行的时候会被排除(不执行指定的task) |

  



 
