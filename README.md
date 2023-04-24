# 《Windows 内核安全编程技术实践》

<div align=center>
<img width="150" src="https://user-images.githubusercontent.com/52789403/201465673-01dd7d47-7092-4523-b828-8af16030b979.png" />
</div>

**作者：** 王瑞<br>
**页数：** 798页<br>
**开本：** 16开<br>
**装帧：** 平装<br>
**登记号：** 国作登字-2023-L-00070201<br>

## 知识产权声明

该作品已在中国版权保护中心（国家版权局）申请登记，受《中华人民共和国著作权法》的保护，作者以著作权人身份依法享有，发表权、署名权、修改权、保护作品完整权、复制权、发行权、出租权、展览权、表演权、放映权、广播权、信息网络传播权、摄制权、改编权、翻译权、汇编权，及著作权人依法享有的其他合法权益。

## 封面设计


![logo](https://user-images.githubusercontent.com/52789403/233877760-ca55b957-448a-4d08-903c-be71f189f0cb.PNG)

## 书籍概述

Windows 内核安全编程技术实践，是一本于2023年3月4日创作完成，并于3月6日在北京首次发表的图书作品，著作权人是王瑞。本书图文并茂、深入浅出、案例丰富，是Windows内核开发工程师的参考资料，也可供信息安全，软件工程等相关专业本科及以上在校生学习参考。本书是近年来少见的关于揭秘AntiRootkit反内核工具实现细节的相关书籍。

## 内容简介

Windows 内核安全编程技术实践（纯64位），由作者多年技术积累编写而成，该书由浅入深、循序渐进地介绍了 Windows 内核程序的开发方法与调试技巧。书如其名揭秘 Anti Rootkit 反内核工具核心原理与技术实现细节，本书最大的特色在于每一节的例子都是经过精挑细选的，具有很强的针对性。不同于市面上的多数 内核开发 系列丛书，本书是以内核安全角度为切入点，以实战角度出发，力求让读者通过亲自动手实验，掌握各类 Windows 内核安全编程的相关技巧，学到尽可能多的 Windows 底层知识。 本书适用于中、高级系统安全工程师，同时也可用做高校计算机专业操作系统开发实验课的补充教材。

## 书籍目录

 - 第一章：环境配置篇
   - 1.1 配置驱动开发环境
   - 1.2 配置驱动开发模板
   - 1.3 配置驱动双机调试
   - 1.4 测试模式过DSE签名

 - 第二章：基础知识篇
   - 2.1 内核中的链表与结构体
   - 2.2 内核中的自旋锁结构
   - 2.3 内核字符串转换方法
   - 2.4 内核字符串拷贝与比较
   - 2.5 探索DRIVER驱动对象
   - 2.6 内核使用IO/DPC定时器

 - 第三章：内核驱动通信篇
   - 3.1 驱动程序与应用层简单通信
   - 3.2 应用DeviceIoContro开发模板
   - 3.3 应用DeviceIoContro模板精讲
   - 3.4 通过SystemBuf与内核层通信
   - 3.5 通过ReadFile与内核层通信
   - 3.6 通过PIPE管道与内核层通信
   - 3.7 通过Async反向与内核通信
   - 3.8 运用MDL映射实现多次通信
   - 3.9 通过应用层堆实现多次通信
   - 3.10 基于事件同步的反向通信

 - 第四章：内核驱动读写篇
   - 4.1 内核远程堆分配与销毁
   - 4.2 内核CR3切换读写内存
   - 4.3 内核MDL读写进程内存
   - 4.4 通过内存拷贝读写内存
   - 4.5 内核R3与R0内存映射拷贝
   - 4.6 内核进程汇编与反汇编
   - 4.7 内核解析内存四级页表
   - 4.8 内核读写内存浮点数
   - 4.9 内核读写内存多级偏移
   - 4.10 内核物理内存寻址读写

 - 第五章：内核SSDT枚举篇
   - 5.1 内核枚举SSDT表基址
   - 5.2 内核枚举SSSDT表基址

 - 第六章：内核进程线程篇
   - 6.1 内核中进程与句柄互转
   - 6.2 内核中枚举进线程与模块
   - 6.3 监控进程与线程对象操作
   - 6.4 内核监控进程与线程创建
   - 6.5 内核DKOM实现进程隐藏
   - 6.6 内核中实现Dump进程转储
   - 6.7 内核遍历进程VAD结构体
   - 6.8 运用VAD隐藏R3内存思路
   - 6.9 内核摘链DKOM进程隐藏
   - 6.10 内核无痕隐藏自身分析
   - 6.11 内核强制结束进程运行

 - 第七章：内核模块篇
   - 7.1 内核判断驱动加载状态
   - 7.2 内核取ntoskrnl模块基地址
   - 7.3 内核取应用层模块基地址
   - 7.4 内核通过PEB取进程参数
   - 7.5 断链隐藏驱动程序自身
   - 7.6 内核特征码搜索函数封装
   - 7.7 内核LDE引擎计算汇编长度
   - 7.8 内核层InlineHook挂钩函数
   - 7.9 摘除InlineHook内核钩子
   - 7.10 取进程模块的函数地址

 - 第八章：内核枚举篇
   - 8.1 内核枚举IoTimer定时器
   - 8.2 内核枚举DpcTimer定时器
   - 8.3 内核枚举PspCidTable句柄表
   - 8.4 内核枚举Minifilter微过滤驱动
   - 8.5 内核枚举LoadImage映像回调
   - 8.6 内核枚举Registry注册表回调
   - 8.7 内核枚举进线程ObCall回调

 - 第九章：内核监控篇
   - 9.1 内核监控进程与线程回调
   - 9.2 内核注册并监控对象回调
   - 9.3 内核监视LoadImage映像回调
   - 9.4 内核运用LoadImage屏蔽驱动
   - 9.5 内核监控Register注册表回调
   - 9.6 内核监控FileObject文件回调

 - 第十章：内核网络通信篇
   - 10.1 内核封装WSK网络通信接口
   - 10.2 内核封装TDI网络通信接口
   - 10.3 内核封装WFP防火墙入门

 - 第十一章：内核PE结构篇
   - 11.1 内核特征扫描PE代码段
   - 11.2 内核解析PE结构导出表
   - 11.3 内核解析PE结构节表
   - 11.4 内核PE结构VA与FOA转换
   - 11.5 内核实现SSDT挂钩与摘钩
   - 11.6 内核扫描SSDT挂钩状态
   - 11.7 PE导出函数与RVA转换
   - 11.8 内核RIP劫持实现DLL注入
   - 11.9 内核远程线程实现DLL注入
   - 11.10 内核LoadLibrary实现DLL注入
   - 11.11 内核ShellCode实现线程注入

 - 第十二章：内核文件与注册表篇
   - 12.1 内核文件读写系列函数
   - 12.2 内核解锁与强删文件
   - 12.3 内核遍历文件或目录
   - 12.4 文件微过滤驱动入门
   - 12.5 内核注册表增删改查

 - 附录
 - 参考文献
