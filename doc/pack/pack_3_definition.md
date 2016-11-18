## 打包（pack）操作定义

打包（pack）操作的定义：运行`lkp pack <benchmark name>`命令，自动地进行的一系列操作，包括针对不同的`Benchmark`各自给定的网址（一般是官网下载网址，或者类似SourceForge镜像站的下载地址），使用`wget`命令下载网址所给压缩包或者二进制包（默认暂存于临时目录`/tmp`下），然后进行解压，并且按照指定的方式（可配置）进行编译，最后把该`Benchmark`运行所需的所有文件移动到汇总的存储目录（默认是系统根目录下的`/lkp/benchmark`目录中）并使用`gzip | cpio`命令进行打包。