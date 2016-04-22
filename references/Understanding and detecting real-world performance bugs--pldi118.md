## 总结：

主要就是针对几个主流的文件系统，量化了一些分类指标，再进行对比分析。主要可参考之处在其如何进行分类，即文中的几个classification table，对于之后进行性能指标的设定和分析会比较有参考价值。


##主要内容：

性能bug指效率低下的代码段所带来的性能降低和资源浪费问题。在未来硬件性能受限、软件系统日益复杂、能源问题愈加严重的情况下，性能bug的危害性十分巨大。但是人们往往忽视性能bug，认为性能问题只跟编译器和硬件有关。

本文选取109个随机抽查的bug和五套开源软件套装，进行如下研究：指导如何避免bug，**指导如何检测性能**，指导如何检测bug，指导如何修复bug，与功能性bug的比较

https://www.cs.wisc.edu/users/shanlu/performance-bugs