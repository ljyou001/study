# Linux性能优化实战学习笔记

   * [Linux性能优化实战学习笔记]()
      * [<a href="https://time.geekbang.org/column/article/69618" rel="nofollow">02 | 基础篇：到底应该怎么理解“平均负载”？</a>](https://time.geekbang.org/column/article/69618)
         * [平均负载]()
         * [平均负载为多少时合理]()
         * [uptime]()
         * [小白三板斧]()
            * [1. uptime 查看平均负载的变化情况]()
            * [2. mpstat 查看 CPU 使用率的变化情况]()
            * [3. pidstat 查找罪魁祸首]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/69859" rel="nofollow">03 | 基础篇：经常说的 CPU 上下文切换是什么意思？（上）</a>](https://time.geekbang.org/column/article/69859)
         * [线程与进程最大的区别]()
         * [中断上下文切换]()
      * [<a href="https://time.geekbang.org/column/article/70077" rel="nofollow">04 | 基础篇：经常说的 CPU 上下文切换是什么意思？（下）</a>](https://time.geekbang.org/column/article/70077)
         * [vmstat 查询系统总体的上下文切换情况]()
         * [pidstat -w 查看每个进程的详细情况]()
         * [观察中断的变化情况]()
         * [每秒上下文切换多少次才算正常呢？]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/70476" rel="nofollow">05 | 基础篇：某个应用的CPU使用率居然达到100\x，我该怎么办？</a>](https://time.geekbang.org/column/article/70476)
         * [查看 CPU 使用率]()
         * [CPU 使用率相关的重要指标]()
         * [CPU 使用率过高怎么办？]()
            * [perf 适合在第一时间分析进程的 CPU 问题]()
               * [两种最常见方法]()
      * [<a href="https://time.geekbang.org/column/article/70822" rel="nofollow">06 | 案例篇：系统的 CPU 使用率很高，但为啥却找不到高 CPU 的应用？</a>](https://time.geekbang.org/column/article/70822)
         * [pstree 查找一个进程的父进程]()
         * [分析 CPU 使用率的工具]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/71064" rel="nofollow">07 | 案例篇：系统中出现大量不可中断进程和僵尸进程怎么办？（上）</a>](https://time.geekbang.org/column/article/71064)
         * [TOP 命令]()
         * [dstat 性能工具]()
      * [<a href="https://time.geekbang.org/column/article/71382" rel="nofollow">08 | 案例篇：系统中出现大量不可中断进程和僵尸进程怎么办？（下）</a>](https://time.geekbang.org/column/article/71382)
         * [iowait 分析]()
         * [strace 正是最常用的跟踪进程系统调用的工具]()
         * [僵尸进程]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/71868" rel="nofollow">09 | 基础篇：怎么理解Linux软中断？</a>](https://time.geekbang.org/column/article/71868)
         * [查看软中断和内核线程]()
         * [小结]()
      * [10 | 案例篇：系统的软中断CPU使用率升高，我该怎么办？]()
         * [观察中断次数的变化速率]()
         * [sar 用来查看系统的网络收发情况]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/72685" rel="nofollow">11 | 套路篇：如何迅速分析出系统CPU的瓶颈在哪里？</a>](https://time.geekbang.org/column/article/72685)
      * [<a href="https://time.geekbang.org/column/article/73151" rel="nofollow">12 | 套路篇：CPU 性能优化的几个思路</a>](https://time.geekbang.org/column/article/73151)
         * [怎么评估性能优化的效果？]()
         * [应用程序优化]()
         * [系统优化]()
      * [<a href="https://time.geekbang.org/column/article/73738" rel="nofollow">14 | 答疑（二）：如何用perf工具分析Java程序？</a>](https://time.geekbang.org/column/article/73738)
         * [性能优化书籍和参考资料推荐]()
      * [<a href="https://time.geekbang.org/column/article/74272" rel="nofollow">15 | 基础篇：Linux内存是怎么工作的？</a>](https://time.geekbang.org/column/article/74272)
         * [如何查看内存使用情况]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/74633" rel="nofollow">16 | 基础篇：怎么理解内存中的Buffer和Cache？</a>](https://time.geekbang.org/column/article/74633)
      * [<a href="https://time.geekbang.org/column/article/75242" rel="nofollow">17 | 案例篇：如何利用系统缓存优化程序的运行效率？</a>](https://time.geekbang.org/column/article/75242)
         * [缓存命中率]()
            * [cachestat 和 cachetop ，是查看系统缓存命中情况的工具]()
               * [没有成功！]()
      * [<a href="https://time.geekbang.org/column/article/75670" rel="nofollow">18 | 案例篇：内存泄漏了，我该如何定位和处理？</a>](https://time.geekbang.org/column/article/75670)
         * [memleak 专门用来检测内存泄漏的工具]()
      * [<a href="https://time.geekbang.org/column/article/75797" rel="nofollow">19 | 案例篇：为什么系统的Swap变高了（上）</a>](https://time.geekbang.org/column/article/75797)
         * [kswapd0]()
         * [numactl 命令]()
      * [<a href="https://time.geekbang.org/column/article/75973" rel="nofollow">20 | 案例篇：为什么系统的Swap变高了？（下）</a>](https://time.geekbang.org/column/article/75973)
      * [<a href="https://time.geekbang.org/column/article/76460" rel="nofollow">21 | 套路篇：如何“快准狠”找到系统内存的问题？</a>](https://time.geekbang.org/column/article/76460)
         * [内存性能指标（详见文中插图）]()
         * [内存性能工具]()
         * [常见的优化思路]()
      * [<a href="https://time.geekbang.org/column/article/76876" rel="nofollow">23 | 基础篇：Linux 文件系统是怎么工作的？</a>](https://time.geekbang.org/column/article/76876)
         * [虚拟文件系统]()
         * [文件读写方式的各种差异，导致 I/O 的分类多种多样]()
         * [性能观测]()
      * [<a href="https://time.geekbang.org/column/article/77010" rel="nofollow">24 | 基础篇：Linux 磁盘I/O是怎么工作的（上）</a>](https://time.geekbang.org/column/article/77010)
         * [I/O 栈]()
      * [<a href="https://time.geekbang.org/column/article/77511" rel="nofollow">25 | 基础篇：Linux 磁盘I/O是怎么工作的（下）</a>](https://time.geekbang.org/column/article/77511)
         * [磁盘性能指标]()
      * [<a href="https://time.geekbang.org/column/article/77885" rel="nofollow">26 | 案例篇：如何找出狂打日志的“内鬼”？</a>](https://time.geekbang.org/column/article/77885)
      * [<a href="https://time.geekbang.org/column/article/78409" rel="nofollow">27 | 案例篇：为什么我的磁盘I/O延迟很高？</a>](https://time.geekbang.org/column/article/78409)
      * [<a href="https://time.geekbang.org/column/article/79001" rel="nofollow">30 | 套路篇：如何迅速分析出系统I/O的瓶颈在哪里？</a>](https://time.geekbang.org/column/article/79001)
      * [<a href="https://time.geekbang.org/column/article/79368" rel="nofollow">31 | 套路篇：磁盘 I/O 性能优化的几个思路</a>](https://time.geekbang.org/column/article/79368)
         * [I/O 基准测试]()
      * [<a href="https://time.geekbang.org/column/article/79734" rel="nofollow">32 | 答疑（四）：阻塞、非阻塞 I/O 与同步、异步 I/O 的区别和联系</a>](https://time.geekbang.org/column/article/79734)
      * [<a href="https://time.geekbang.org/column/article/81057" rel="nofollow">34 | 关于 Linux 网络，你必须知道这些（下）</a>](https://time.geekbang.org/column/article/81057)
         * [性能指标]()
         * [网络配置]()
            * [1. 网络接口的状态标志]()
            * [2. MTU 的大小]()
            * [3. 网络接口的 IP 地址、子网以及 MAC 地址]()
            * [4. 网络收发的字节数、包数、错误数以及丢包情况]()
         * [套接字信息]()
         * [协议栈统计信息]()
         * [网络吞吐和 PPS]()
            * [查看网卡速度]()
         * [连通性和延时]()
      * [<a href="https://time.geekbang.org/column/article/81268" rel="nofollow">35 | 基础篇：C10K 和 C1000K 回顾</a>](https://time.geekbang.org/column/article/81268)
         * [I/O 模型优化]()
            * [第一种，使用非阻塞 I/O 和水平触发通知，比如使用 select 或者 poll]()
            * [第二种，使用非阻塞 I/O 和边缘触发通知，比如 epoll]()
            * [第三种，使用异步 I/O（Asynchronous I/O，简称为 AIO）]()
         * [工作模型优化]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/81497" rel="nofollow">36 | 套路篇：怎么评估系统的网络性能？</a>](https://time.geekbang.org/column/article/81497)
         * [各协议层的性能测试]()
            * [转发性能]()
            * [TCP/UDP 性能]()
               * [iperf]()
            * [HTTP 性能]()
            * [应用负载性能]()
      * [<a href="https://time.geekbang.org/column/article/81850" rel="nofollow">37 | 案例篇：DNS 解析时快时慢，我该怎么办？</a>](https://time.geekbang.org/column/article/81850)
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/82321" rel="nofollow">38 | 案例篇：怎么使用 tcpdump 和 Wireshark 分析网络流量？</a>](https://time.geekbang.org/column/article/82321)
      * [<a href="https://time.geekbang.org/column/article/82833" rel="nofollow">40 | 案例篇：网络请求延迟变大了，我该怎么办？</a>](https://time.geekbang.org/column/article/82833)
      * [<a href="https://time.geekbang.org/column/article/83189" rel="nofollow">41 | 案例篇：如何优化 NAT 性能？（上）</a>](https://time.geekbang.org/column/article/83189)
      * [<a href="https://time.geekbang.org/column/article/83520" rel="nofollow">42 | 案例篇：如何优化 NAT 性能？（下）</a>](https://time.geekbang.org/column/article/83520)
      * [<a href="https://time.geekbang.org/column/article/83783" rel="nofollow">43 | 套路篇：网络性能优化的几个思路（上）</a>](https://time.geekbang.org/column/article/83783)
         * [为了提高网络的吞吐量，你通常需要调整这些缓冲区的大小]()
         * [除此之外，套接字接口还提供了一些配置选项，用来修改网络连接的行为：]()
      * [<a href="https://time.geekbang.org/column/article/84003" rel="nofollow">44 | 套路篇：网络性能优化的几个思路（下）</a>](https://time.geekbang.org/column/article/84003)
         * [网络性能优化]()
            * [传输层]()
               * [TCP 协议的优化]()
               * [UDP 的优化]()
            * [网络层]()
               * [第一种，从路由和转发的角度出发，你可以调整下面的内核选项]()
               * [第二种，从分片的角度出发，最主要的是调整 MTU（Maximum Transmission Unit）的大小。]()
               * [第三种，从 ICMP 的角度出发，为了避免 ICMP 主机探测、ICMP Flood 等各种网络问题，你可以通过内核选项，来限制 ICMP 的行为。]()
            * [链路层]()
               * [由于网卡收包后调用的中断处理程序（特别是软中断），需要消耗大量的 CPU。所以，将这些中断处理程序调度到不同的 CPU 上执行，就可以显著提高网络吞吐量。这通常可以采用下面两种方法。]()
               * [现在的网卡都有很丰富的功能，原来在内核中通过软件处理的功能，可以卸载到网卡中，通过硬件来执行。]()
               * [对于网络接口本身，也有很多方法，可以优化网络的吞吐量]()
               * [C10M]()
         * [小结]()
      * [<a href="https://time.geekbang.org/column/article/86330" rel="nofollow">49 | 案例篇：内核线程 CPU 利用率太高，我该怎么办？</a>](https://time.geekbang.org/column/article/86330)
         * [火焰图]()
      * [<a href="https://time.geekbang.org/column/article/86490" rel="nofollow">50 | 案例篇：动态追踪怎么用？（上）</a>](https://time.geekbang.org/column/article/86490)
         * [动态追踪]()
            * [ftrace]()
      * [<a href="https://time.geekbang.org/column/article/86710" rel="nofollow">51 | 案例篇：动态追踪怎么用？（下）</a>](https://time.geekbang.org/column/article/86710)
         * [perf]()
         * [eBPF 和 BCC]()
         * [SystemTap 和 sysdig]()
         * [如何选择追踪工具]()
      * [<a href="https://time.geekbang.org/column/article/87980" rel="nofollow">53 | 套路篇：系统监控的综合思路</a>](https://time.geekbang.org/column/article/87980)
         * [USE 法]()
         * [监控系统]()
      * [<a href="https://time.geekbang.org/column/article/88423" rel="nofollow">54 | 套路篇：应用监控的一般思路</a>](https://time.geekbang.org/column/article/88423)
         * [RED原则]()
         * [指标监控]()
         * [日志监控]()
      * [<a href="https://time.geekbang.org/column/article/88667" rel="nofollow">55 | 套路篇：分析性能问题的一般步骤</a>](https://time.geekbang.org/column/article/88667)
      * [<a href="https://time.geekbang.org/column/article/89278" rel="nofollow">56 | 套路篇：优化性能问题的一般方法</a>](https://time.geekbang.org/column/article/89278)
      * [<a href="https://time.geekbang.org/column/article/89306" rel="nofollow">57 | 套路篇：Linux 性能工具速查</a>](https://time.geekbang.org/column/article/89306)
      * [<a href="https://time.geekbang.org/column/article/80829" rel="nofollow">加餐（一） | 书单推荐：性能优化和Linux 系统原理</a>](https://time.geekbang.org/column/article/80829)
      * [<a href="https://time.geekbang.org/column/article/84619" rel="nofollow">加餐（二） | 书单推荐：网络原理和 Linux 内核实现</a>](https://time.geekbang.org/column/article/84619)

目录生成 [源码：gh-md-toc](https://github.com/ekalinin/github-markdown-toc) | [在线地址](https://sleepeatcode.com/ghtoc)


## [02 | 基础篇：到底应该怎么理解“平均负载”？](https://time.geekbang.org/column/article/69618)

### 平均负载

- 是指单位时间内，系统处于**可运行状态**和**不可中断状态**的平均进程数，也就是**平均活跃进程数**，它和 CPU 使用率并没有直接关系。

### 平均负载为多少时合理
- 首先你要知道系统有几个 CPU

```cmd
$ grep 'model name' /proc/cpuinfo | wc -l
```

- 当平均负载比 CPU 个数还大的时候，系统已经出现了过载

### uptime

```cmd
02:34:03              //当前时间
up 2 days, 20:14      //系统运行时间
1 user                //正在登录用户数
```

- 最后三个数，依次则是过去 1 分钟、5 分钟、15 分钟的平均负载（Load Average）

### 小白三板斧

#### 1. uptime 查看平均负载的变化情况

```cmd
# -d 参数表示高亮显示变化的区域
$ watch -d uptime
...,  load average: 1.00, 0.75, 0.39
```

#### 2. mpstat 查看 CPU 使用率的变化情况

```cmd
# -P ALL 表示监控所有CPU，后面数字5表示间隔5秒后输出一组数据
$ mpstat -P ALL 5
```

#### 3. pidstat 查找罪魁祸首

```cmd
# 间隔5秒后输出一组数据
$ pidstat -u 5 1
```

### 小结

- 平均负载提供了一个快速查看系统整体性能的手段，反映了整体的负载情况。但只看平均负载本身，我们并不能直接发现，到底是哪里出现了瓶颈。
 
 - 平均负载高有可能是 CPU 密集型进程导致的；
 - 平均负载高并不一定代表 CPU 使用率高，还有可能是 I/O 更繁忙了；
 - 当发现负载高的时候，你可以使用 mpstat、pidstat 等工具，辅助分析负载的来源。

## [03 | 基础篇：经常说的 CPU 上下文切换是什么意思？（上）](https://time.geekbang.org/column/article/69859)

- 过多的上下文切换，会把 CPU 时间消耗在寄存器、内核栈以及虚拟内存等数据的保存和恢复上，缩短进程真正运行的时间，成了系统性能大幅下降的一个元凶。

- CPU 寄存器和程序计数器（Program Counter，PC）也被叫做 CPU 上下文

- 根据任务的不同，CPU 的上下文切换就可以分为几个不同的场景
  - 进程上下文切换
  - 线程上下文切换
  - 中断上下文切换

### 线程与进程最大的区别

- **线程是调度的基本单位，而进程则是资源拥有的基本单位**。说白了，所谓内核中的任务调度，实际上的调度对象是线程；而进程只是给线程提供了虚拟内存、全局变量等资源。
  
  - 当进程只有一个线程时，可以认为进程就等于线程。
  - 当进程拥有多个线程时，这些线程会共享相同的虚拟内存和全局变量等资源。这些资源在上下文切换时是不需要修改的。
  - 另外，线程也有自己的私有数据，比如栈和寄存器等，这些在上下文切换时也是需要保存的。

### 中断上下文切换

- 为了快速响应硬件的事件，**中断处理会打断进程的正常调度和执行**，转而调用中断处理程序，响应设备事件。

- 跟进程上下文不同，中断上下文切换并不涉及到进程的用户态。所以，即便中断过程打断了一个正处在用户态的进程，也不需要保存和恢复这个进程的虚拟内存、全局变量等用户态资源。中断上下文，其实只包括内核态中断服务程序执行所必需的状态，包括 CPU 寄存器、内核堆栈、硬件中断参数等。

- 对同一个 CPU 来说，中断处理比进程拥有更高的优先级，所以中断上下文切换并不会与进程上下文切换同时发生。同样道理，由于中断会打断正常进程的调度和执行，所以大部分中断处理程序都短小精悍，以便尽可能快的执行结束。

## [04 | 基础篇：经常说的 CPU 上下文切换是什么意思？（下）](https://time.geekbang.org/column/article/70077)

### vmstat 查询系统总体的上下文切换情况

- vmstat 是一个常用的系统性能分析工具，主要用来分析
  - 系统的内存使用情况
  - CPU 上下文切换和中断的次数

```cmd
# 每隔5秒输出1组数据
$ vmstat 5

# 每隔1秒输出2组数据
$ vmstat 1 2
```

需要特别关注的四列内容：

- cs（context switch）是每秒上下文切换的次数。
- in（interrupt）则是每秒中断的次数。
- r（Running or Runnable）是就绪队列的长度，也就是正在运行和等待 CPU 的进程数。
- b（Blocked）则是处于不可中断睡眠状态的进程数。

### pidstat -w 查看每个进程的详细情况

```cmd
# 每隔5秒输出1组数据
$ pidstat -w 5
```

重点关注两列

- cswch ，表示每秒自愿上下文切换（voluntary context switches）的次数
- nvcswch ，表示每秒非自愿上下文切换（non voluntary context switches）的次数

> - **自愿上下文切换，是指进程无法获取所需资源，导致的上下文切换**。比如说， I/O、内存等系统资源不足时，就会发生自愿上下文切换。

> - **非自愿上下文切换，则是指进程由于时间片已到等原因，被系统强制调度，进而发生的上下文切换**。比如说，大量进程都在争抢 CPU 时，就容易发生非自愿上下文切换。


```cmd
# -w参数表示输出进程切换指标，而-u参数则表示输出CPU使用指标
$ pidstat -w -u 1
```

```cmd
# -wt 参数表示输出线程的上下文切换指标
$ pidstat -wt 1
```

### 观察中断的变化情况

```cmd
# -d 参数表示高亮显示变化的区域
$ watch -d cat /proc/interrupts
```

- **重调度中断**（RES），这个中断类型表示，唤醒空闲状态的 CPU 来调度新的任务运行。这是多处理器系统（SMP）中，调度器用来分散任务到不同 CPU 的机制，通常也被称为**处理器间中断**（Inter-Processor Interrupts，IPI）。

### 每秒上下文切换多少次才算正常呢？

- **这个数值其实取决于系统本身的 CPU 性能。**如果系统的上下文切换次数比较稳定，那么从**数百**到**一万以内**，都应该算是正常的。

- 但当上下文切换次数**超过一万次**，或者切换次数出现数量级的增长时，就很可能已经出现了性能问题。

- 根据上下文切换的类型，分析原因：
 - 自愿上下文切换变多了，说明进程都在等待资源，有可能发生了 I/O 等其他问题；
 - 非自愿上下文切换变多了，说明进程都在被强制调度，也就是都在争抢 CPU，说明 CPU 的确成了瓶颈；
 - 中断次数变多了，说明 CPU 被中断处理程序占用，还需要通过查看 /proc/interrupts 文件来分析具体的中断类型。

### 小结
- 可以借助 vmstat 、 pidstat 和 /proc/interrupts 等工具来排查性能问题。

## [05 | 基础篇：某个应用的CPU使用率居然达到100%，我该怎么办？](https://time.geekbang.org/column/article/70476)

- **性能分析工具给出的都是间隔一段时间的平均 CPU 使用率，所以要注意间隔时间的设置**，特别是用多个工具对比分析时，你一定要保证它们用的是相同的间隔时间。

### 查看 CPU 使用率

- top 显示了系统总体的 CPU 和内存使用情况，以及各个进程的资源使用情况。
- ps 则只显示了每个进程的资源使用情况。

###  CPU 使用率相关的重要指标

- user（通常缩写为 us），代表用户态 CPU 时间。注意，它不包括下面的 nice 时间，但包括了 guest 时间。
- nice（通常缩写为 ni），代表低优先级用户态 CPU 时间，也就是进程的 nice 值被调整为 1-19 之间时的 CPU 时间。这里注意，nice 可取值范围是 -20 到 19，数值越大，优先级反而越低。
- system（通常缩写为 sys），代表内核态 CPU 时间。
- idle（通常缩写为 id），代表空闲时间。注意，它不包括等待 I/O 的时间（iowait）。
- iowait（通常缩写为 wa），代表等待 I/O 的 CPU 时间。
- irq（通常缩写为 hi），代表处理硬中断的 CPU 时间。
- softirq（通常缩写为 si），代表处理软中断的 CPU 时间。
- steal（通常缩写为 st），代表当系统运行在虚拟机中的时候，被其他虚拟机占用的 CPU 时间。
- guest（通常缩写为 guest），代表通过虚拟化运行其他操作系统的时间，也就是运行虚拟机的 CPU 时间。
- guest_nice（通常缩写为 gnice），代表以低优先级运行虚拟机的时间。

### CPU 使用率过高怎么办？

- GDB（The GNU Project Debugger）， 功能强大的程序调试利器。
  - GDB 并不适合在性能分析的早期应用。
  - GDB 只适合用在性能分析的后期，当你找到了出问题的大致函数后，线下再借助它来进一步调试函数内部的问题。

#### perf 适合在第一时间分析进程的 CPU 问题

- perf 是 Linux 2.6.31 以后内置的性能分析工具。
- 它以性能事件采样为基础
  - 不仅可以分析系统的各种事件和内核性能
  - 还可以用来分析指定应用程序的性能问题

##### 两种最常见方法

```cmd
$ perf top
```

输出结果中，第一行包含三个数据，分别是

- 采样数（Samples）
- 事件类型（event）
- 事件总数量（Event count）

**采样数需要我们特别注意**。如果采样数过少（比如只有十几个），那下面的排序和百分比就没什么实际参考价值了。

再往下看是一个表格式样的数据，每一行包含四列，分别是：

- 第一列 Overhead ，是该符号的性能事件在所有采样中的比例，用百分比来表示。
- 第二列 Shared ，是该函数或指令所在的动态共享对象（Dynamic Shared Object），如内核、进程名、动态链接库名、内核模块名等。
- 第三列 Object ，是动态共享对象的类型。比如 [.] 表示用户空间的可执行程序、或者动态链接库，而 [k] 则表示内核空间。
- 最后一列 Symbol 是符号名，也就是函数名。当函数名未知时，用十六进制的地址来表示。

```cmd
perf record 和 perf report
```

perf top 虽然实时展示了系统的性能信息，但它的缺点是并不保存数据，也就无法用于离线或者后续的分析。而 perf record 则提供了保存数据的功能，保存后的数据，需要你用 perf report 解析展示。

```cmd
# 按Ctrl+C终止采样
$ perf record -g

# 展示类似于perf top的报告
$ perf report
```

在实际使用中，我们还经常为 perf top 和 perf record 加上 -g 参数，开启调用关系的采样，方便我们根据调用链来分析性能问题。

## [06 | 案例篇：系统的 CPU 使用率很高，但为啥却找不到高 CPU 的应用？](https://time.geekbang.org/column/article/70822)

### pstree 查找一个进程的父进程

```cmd
$ pstree | grep stress
```

### 分析 CPU 使用率的工具

- perf
- [execsnoop](https://github.com/brendangregg/perf-tools/blob/master/execsnoop)
 - 一个专为短时进程设计的工具。
 - 它通过 ftrace 实时监控进程的 exec() 行为，并输出短时进程的基本信息，包括进程 PID、父进程 PID、命令行参数以及执行的结果。

### 小结

碰到常规问题无法解释的 CPU 使用率情况时，首先要想到有可能是短时应用导致的问题，比如有可能是下面这两种情况。

- 第一，应用里直接调用了其他二进制程序，这些程序通常运行时间比较短，通过 top 等工具也不容易发现。
- 第二，应用本身在不停地崩溃重启，而启动过程的资源初始化，很可能会占用相当多的 CPU。

对于这类进程，我们可以用 pstree 或者 execsnoop 找到它们的父进程，再从父进程所在的应用入手，排查问题的根源。

## [07 | 案例篇：系统中出现大量不可中断进程和僵尸进程怎么办？（上）](https://time.geekbang.org/column/article/71064)

### TOP 命令

S 列（也就是 Status 列）表示进程的状态

- **R** 是 Running 或 Runnable 的缩写，表示进程在 CPU 的就绪队列中，正在运行或者正在等待运行。
- **D** 是 Disk Sleep 的缩写，也就是不可中断状态睡眠（Uninterruptible Sleep），一般表示进程正在跟硬件交互，并且交互过程不允许被其他进程或中断打断。
- **Z** 是 Zombie 的缩写，如果你玩过“植物大战僵尸”这款游戏，应该知道它的意思。它表示僵尸进程，也就是进程实际上已经结束了，但是父进程还没有回收它的资源（比如进程的描述符、PID 等）。
- **S** 是 Interruptible Sleep 的缩写，也就是可中断状态睡眠，表示进程因为等待某个事件而被系统挂起。当进程等待的事件发生时，它会被唤醒并进入 
- **R** 状态。
- **I** 是 Idle 的缩写，也就是空闲状态，用在不可中断睡眠的内核线程上。前面说了，硬件交互导致的不可中断进程用 D 表示，但对某些内核线程来说，它们有可能实际上并没有任何负载，用 Idle 正是为了区分这种情况。要注意，D 状态的进程会导致平均负载升高， I 状态的进程却不会。
- **T 或者 t** 也就是 Stopped 或 Traced 的缩写，表示进程处于暂停或者跟踪状态。
- **X** 也就是 Dead 的缩写，表示进程已经消亡，所以你不会在 top 或者 ps 命令中看到它。

### dstat 性能工具

- 它吸收了 vmstat、iostat、ifstat 等几种工具的优点
- 可以同时观察系统的 CPU、磁盘 I/O、网络以及内存使用情况

## [08 | 案例篇：系统中出现大量不可中断进程和僵尸进程怎么办？（下）](https://time.geekbang.org/column/article/71382)

### iowait 分析

- 推荐工具 dstat

```cmd
# 间隔1秒输出10组数据
$ dstat 1 10
```

根据进程号排查

```cmd
# -d 展示 I/O 统计数据，-p 指定进程号，间隔 1 秒输出 3 组数据
$ pidstat -d -p 4344 1 3
```

没有发现异常，去掉进程号，观察所有进程的 I/O 使用情况

```cmd
# 间隔 1 秒输出多组数据 (这里是 20 组)
$ pidstat -d 1 20
```

### strace 正是最常用的跟踪进程系统调用的工具

```cmd
# -p 参数指定 PID 号
$ strace -p 6082
```

检查进程状态是否正常

```cmd
$ ps aux | grep 6082
```

### 僵尸进程

pstree 查找父进程

```cmd
# -a 表示输出命令行选项
# p表PID
# s表示指定进程的父进程
$ pstree -aps 3084
```

### 小结

- iowait 高不一定代表 I/O 有性能瓶颈。
- 当系统中只有 I/O 类型的进程在运行时，iowait 也会很高，但实际上，磁盘的读写远没有达到性能瓶颈的程度。
- 碰到 iowait 升高时，需要先用 dstat、pidstat 等工具，确认是不是磁盘 I/O 的问题，然后再找是哪些进程导致了 I/O。

## [09 | 基础篇：怎么理解Linux软中断？](https://time.geekbang.org/column/article/71868)

### 查看软中断和内核线程

- /proc/softirqs 提供了软中断的运行情况
- /proc/interrupts 提供了硬中断的运行情况

查看 /proc/softirqs 文件的内容，你就可以看到各种类型软中断在不同 CPU 上的累积运行次数：

```cmd
$ cat /proc/softirqs
```

- **NET_RX** 表示网络接收中断 
- **NET_TX** 表示网络发送中断
- **TASKLET** 在不同 CPU 上的分布并不均匀。TASKLET 是最常用的软中断实现机制，每个 TASKLET 只运行一次就会结束 ，并且**只在调用它的函数所在的 CPU 上运行**
    - 缺点 
        - **由于只在一个 CPU 上运行导致的调度不均衡**
        - **因为不能在多个 CPU 上并行运行带来了性能限制**
- **TIMER** 定时中断
- **SCHED** 内核调度
- **RCU** RCU 锁


软中断实际上是以内核线程的方式运行的，每个 CPU 都对应一个软中断内核线程，这个软中断内核线程就叫做 ksoftirqd/CPU 编号。那要怎么查看这些线程的运行状况呢？

```cmd
ps aux | grep softirq
```

### 小结

- Linux 中的中断处理程序分为上半部和下半部
 - 上半部对应硬件中断，用来快速处理中断
 - 下半部对应软中断，用来异步处理上半部未完成的工作
- Linux 中的软中断包括网络收发、定时、调度、RCU 锁等各种类型，可以通过查看 /proc/softirqs 来观察软中断的运行情况

## 10 | 案例篇：系统的软中断CPU使用率升高，我该怎么办？

- sar 是一个系统活动报告工具，既可以实时查看系统的当前活动，又可以配置保存和报告历史统计数据。
- hping3 是一个可以构造 TCP/IP 协议数据包的工具，可以对系统进行安全审计、防火墙测试等。
- tcpdump 是一个常用的网络抓包工具，常用来分析各种网络问题。

### 观察中断次数的变化速率

```cmd
$ watch -d cat /proc/softirqs
```

### sar 用来查看系统的网络收发情况

- 不仅可以观察网络收发的吞吐量（BPS，每秒收发的字节数）
- 还可以观察网络收发的 PPS，即每秒收发的网络帧数

```cmd
# -n DEV 表示显示网络收发的报告，间隔1秒输出一组数据
$ sar -n DEV 1
```

sar 的输出界面，从左往右依次是：

- 第一列：表示报告的时间。
- 第二列：IFACE 表示网卡。
- 第三、四列：rxpck/s 和 txpck/s 分别表示每秒接收、发送的网络帧数，也就是 PPS（packet per second 每秒钟有多少数据包经过）。
- 第五、六列：rxkB/s 和 txkB/s 分别表示每秒接收、发送的千字节数，也就是 BPS（每秒钟有多少bit的数据经过）。

BPS * 1024 / PPS = 每个网络帧的字节
如果这个值很小（不足100），就说明是遇到了小包问题

通过 tcpdump 查找小包来源

```cmd
# -i eth0 只抓取eth0网卡，-n不解析协议名和主机名
# tcp port 80表示只抓取tcp协议并且端口号为80的网络帧
$ tcpdump -i eth0 -n tcp port 80
```

### 小结

- 软中断 CPU 使用率（softirq）升高是一种很常见的性能问题。
- 实际生产中，我们遇到的性能瓶颈大多是网络收发类型的软中断，特别是网络接收的软中断。
- 碰到这类问题时，你可以借用 sar、tcpdump 等工具，做进一步分析。

## [11 | 套路篇：如何迅速分析出系统CPU的瓶颈在哪里？](https://time.geekbang.org/column/article/72685)

直接看原文，套路满满，尤其是最后一个图

## [12 | 套路篇：CPU 性能优化的几个思路](https://time.geekbang.org/column/article/73151)

### 怎么评估性能优化的效果？
不要局限在单一维度的指标上，你至少要从应用程序和系统资源这两个维度

- 应用程序的维度，我们可以用**吞吐量和请求延迟**来评估应用程序的性能。
- 系统资源的维度，我们可以用 **CPU 使用率**来评估系统的 CPU 使用情况。

**并不是所有的性能问题都值得优化**
 
 - 找出最重要的、可以最大程度提升性能的问题，从它开始优化。

**性能优化并非没有成本**

### 应用程序优化

- 异步处理
- 善用缓存

### 系统优化

- **CPU 绑定**：把进程绑定到一个或者多个 CPU 上，可以提高 CPU 缓存的命中率，减少跨 CPU 调度带来的上下文切换问题。
- **CPU 独占**：跟 CPU 绑定类似，进一步将 CPU 分组，并通过 CPU 亲和性机制为其分配进程。这样，这些 CPU 就由指定的进程独占，换句话说，不允许其他进程再来使用这些 CPU。
- **优先级调整**：使用 nice 调整进程的优先级，正值调低优先级，负值调高优先级。优先级的数值含义前面我们提到过，忘了的话及时复习一下。在这里，适当降低非核心应用的优先级，增高核心应用的优先级，可以确保核心应用得到优先处理。为进程设置资源限制：使用 Linux cgroups 来设置进程的 CPU 使用上限，可以防止由于某个应用自身的问题，而耗尽系统资源。
- **NUMA（Non-Uniform Memory Access）优化**：支持 NUMA 的处理器会被划分为多个 node，每个 node 都有自己的本地内存空间。NUMA 优化，其实就是让 CPU 尽可能只访问本地内存。
- **中断负载均衡**：无论是软中断还是硬中断，它们的中断处理程序都可能会耗费大量的 CPU。开启 irqbalance 服务或者配置 smp_affinity，就可以把中断处理过程自动负载均衡到多个 CPU 上。

## [14 | 答疑（二）：如何用perf工具分析Java程序？](https://time.geekbang.org/column/article/73738)

- perf 这种动态追踪工具，会给系统带来一定的性能损失。
- vmstat、pidstat 这些直接读取proc 文件系统来获取指标的工具，不会带来性能损失。

### 性能优化书籍和参考资料推荐

**Brendan Gregg 性能优化大师**

- 《Systems Performance: Enterprise and the Cloud》。这本书也出了中文版，名字是《性能之巅：洞悉系统、企业与云计算》。这本书里的性能分析思路以及很多的性能工具，到今天依然适用。
- [Brendan Gregg 个人网站](http://www.brendangregg.com/)
- 特别是 [Linux Performance](http://www.brendangregg.com/linuxperf.html) 这个页面，包含了很多 Linux 性能优化的资料
    - Linux 性能工具图谱
    - 性能分析参考资料
    - 性能优化的演讲视频

## [15 | 基础篇：Linux内存是怎么工作的？](https://time.geekbang.org/column/article/74272)

- 通过减少进程的上下文切换，减少 TLB 的刷新次数，就可以提高 TLB 缓存的使用率，进而提高 CPU 的内存访问性能
- 页的大小只有 4 KB ，导致的另一个问题就是，整个页表会变得非常大。比方说，仅 32 位系统就需要 100 多万个页表项（4GB/4KB），才可以实现整个地址空间的映射
- 为了**解决页表项过多的问题**，Linux 提供了两种机制，也就是**多级页表**和**大页**（HugePage）。
- **大页**：常见的大小有 2MB 和 1GB
- Swap 会导致严重的内存性能问题

管理员可以通过 /proc 文件系统，手动设置进程的 oom_adj ，从而调整进程的 oom_score。oom_adj 的范围是 [-17, 15]，数值越大，表示进程越容易被 OOM 杀死；数值越小，表示进程越不容易被 OOM 杀死，其中 -17 表示禁止 OOM。

```cmd
echo -16 > /proc/$(pidof sshd)/oom_adj
```

### 如何查看内存使用情况

**free** 命令显示整个系统的内存使用情况

```cmd
$ free
```

- 第一列，total 是总内存大小；
- 第二列，used 是已使用内存的大小，包含了共享内存；
- 第三列，free 是未使用内存的大小；
- 第四列，shared 是共享内存的大小；
- 第五列，buff/cache 是缓存和缓冲区的大小；
- 最后一列，available 是新进程可用内存的大小。
    - available 不仅包含未使用内存，还包括了可回收的缓存，所以一般会比未使用内存更大。不过，并不是所有缓存都可以回收，因为有些缓存可能正在使用中。

查看进程的内存使用情况，可以用 **top** 或者 **ps** 等工具

```cmd
# 按下M切换到内存排序
$ top
```

跟内存相关的几列数据，VIRT、RES、SHR、%MEM

- **VIRT** 是进程虚拟内存的大小，只要是进程申请过的内存，即便还没有真正分配物理内存，也会计算在内。
    - 虚拟内存通常并不会全部分配物理内存。从上面的输出，你可以发现每个进程的虚拟内存都比常驻内存大得多。
- **RES** 是常驻内存的大小，也就是进程实际使用的物理内存大小，但不包括 Swap 和共享内存。
- **SHR** 是共享内存的大小，比如与其他进程共同使用的共享内存、加载的动态链接库以及程序的代码段等。
    - 共享内存 SHR 并不一定是共享的，比方说，程序的代码段、非共享的动态链接库，也都算在 SHR 里。当然，SHR 也包括了进程间真正共享的内存。
    - 所以在计算多个进程的内存使用时，不要把所有进程的 SHR 直接相加得出结果。
- **%MEM** 是进程使用物理内存占系统总内存的百分比。

### 小结

- 对普通进程来说，它能看到的其实是内核提供的虚拟内存，这些虚拟内存还需要通过页表，由系统映射为物理内存。
- 当进程通过 malloc() 申请内存后，内存并不会立即分配，而是在首次访问时，才通过缺页异常陷入内核中分配内存。

## [16 | 基础篇：怎么理解内存中的Buffer和Cache？](https://time.geekbang.org/column/article/74633)

清理系统缓存

```cmd
# 清理文件页、目录项、Inodes等各种缓存
$ echo 3 > /proc/sys/vm/drop_caches
```

**Buffer 是对磁盘数据的缓存，而 Cache 是文件数据的缓存，它们既会用在读请求中，也会用在写请求中。**

## [17 | 案例篇：如何利用系统缓存优化程序的运行效率？](https://time.geekbang.org/column/article/75242)

### 缓存命中率

- 命中率越高，表示使用缓存带来的收益越高，应用程序的性能也就越好。

#### cachestat 和 cachetop ，是查看系统缓存命中情况的工具

- cachestat 提供了整个操作系统缓存的读写命中情况。
- cachetop 提供了每个进程的缓存命中情况。

使用 cachestat 和 cachetop 前，我们首先要安装 bcc 软件包

```cmd
$ apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 4052245BD4284CDD
$echo "deb https://repo.iovisor.org/apt/xenial xenial main" | sudo tee /etc/apt/sources.list.d/iovisor.list
$ apt-get update
$ apt-get install -y bcc-tools libbcc-examples linux-headers-$(uname -r)
```

操作完这些步骤，bcc 提供的所有工具就都安装到 /usr/share/bcc/tools 这个目录中了。不过这里提醒你，bcc 软件包默认不会把这些工具配置到系统的 PATH 路径中，所以你得自己手动配置：

```cmd
$ export PATH=$PATH:/usr/share/bcc/tools
```

##### 没有成功！

[使用 snap 安装 bcc](https://snapcraft.io/install/bcc/ubuntu)

安装后进入 /snap/bin

```cmd
$ cd /snap/bin

# 运行时例如
$ ./bcc.filetop -C
```

```cmd
# 查看Linux 内核版本 
cat /proc/version
```

## [18 | 案例篇：内存泄漏了，我该如何定位和处理？](https://time.geekbang.org/column/article/75670)

- 栈内存由系统自动分配和管理
- 堆内存由应用程序自己来分配和管理

### memleak 专门用来检测内存泄漏的工具
- memleak 是 bcc 软件包中的一个工具

## [19 | 案例篇：为什么系统的Swap变高了（上）](https://time.geekbang.org/column/article/75797)

### kswapd0
- 专门的内核线程用来定期回收内存
- kswapd0 定义了三个内存阈值（watermark，也称为水位
    - 页最小阈值（pages_min）
    - 页低阈值（pages_low）
    - 页高阈值（pages_high）
    - 剩余内存，则使用 pages_free 表示。

### numactl 命令
- 来查看处理器在 Node 的分布情况
- 以及每个 Node 的内存使用情况

```cmd
$ numactl --hardware
```

## [20 | 案例篇：为什么系统的Swap变高了？（下）](https://time.geekbang.org/column/article/75973)

Linux 本身支持两种类型的 Swap

- Swap 分区和 
- Swap 文件

降低 Swap 的使用，可以提高系统的整体性能

## [21 | 套路篇：如何“快准狠”找到系统内存的问题？](https://time.geekbang.org/column/article/76460)

套路满满，详见文章配图

### 内存性能指标（详见文中插图）

- 系统
- 进程
- SWAP

### 内存性能工具
- 通过 proc 文件系统，找到了内存指标的来源
- free 查看系统的整体内存和 Swap 使用情况
- top 或 ps，查看进程的内存使用情况
- vmstat 除了可以动态查看内存变化，还可以区分缓存和缓冲区、Swap 换入和换出的内存大小
- cachestat 查看整个系统缓存的读写命中情况
- cachetop 观察每个进程缓存的读写命中情况
- memleak 找到内存泄漏的可疑位置
- sar 发现了缓冲区和 Swap 升高的问题

**为了迅速定位内存问题，通常会先运行几个覆盖面比较大的性能工具，比如 free、top、vmstat、pidstat 等。**

### 常见的优化思路
- 最好禁止 Swap。如果必须开启 Swap，降低 swappiness 的值，减少内存回收时 Swap 的使用倾向。
- 减少内存的动态分配。比如，可以使用内存池、大页（HugePage）等。
- 尽量使用缓存和缓冲区来访问数据。比如，可以使用堆栈明确声明内存空间，来存储需要缓存的数据；或者用 Redis 这类的外部缓存组件，优化数据的访问。
- 使用 cgroups 等方式限制进程的内存使用情况。这样，可以确保系统内存不会被异常进程耗尽。
- 通过 /proc/pid/oom_adj ，调整核心应用的 oom_score。这样，可以保证即使内存紧张，核心应用也不会被 OOM 杀死。

## [23 | 基础篇：Linux 文件系统是怎么工作的？](https://time.geekbang.org/column/article/76876)

- Linux 中一切皆文件。不仅普通的文件和目录，就连块设备、套接字、管道等，也都要通过统一的文件系统来管理。
- 一个文件可以有多个别名

### 虚拟文件系统

- 为了支持各种不同的文件系统，Linux 内核在用户进程和文件系统的中间，又引入了一个抽象层，也就是虚拟文件系统 VFS（Virtual File System）。

### 文件读写方式的各种差异，导致 I/O 的分类多种多样

- 根据**是否利用标准库缓存**，可以把文件 I/O 分为缓冲 I/O 与非缓冲 I/O。
    - 缓冲 I/O，是指利用标准库缓存来加速文件的访问，而标准库内部再通过系统调度访问文件。
    - 非缓冲 I/O，是指直接通过系统调用来访问文件，不再经过标准库缓存。

- 根据**是否利用操作系统的页缓存**，可以把文件 I/O 分为直接 I/O 与非直接 I/O
    - 直接 I/O，是指跳过操作系统的页缓存，直接跟文件系统交互来访问文件
    - 非直接 I/O 正好相反，文件读写时，先要经过系统的页缓存，然后再由内核或额外的系统调用，真正写入磁盘
    - 直接 I/O、非直接 I/O，本质上还是和文件系统交互。如果是在数据库等场景中，你还会看到，跳过文件系统读写磁盘的情况，也就是我们通常所说的**裸 I/O**

- 根据应用程序**是否阻塞自身运行**，可以把文件 I/O 分为阻塞 I/O 和非阻塞 I/O
    - 阻塞 I/O，是指应用程序执行 I/O 操作后，如果没有获得响应，就会阻塞当前线程，自然就不能执行其他任务
    - 非阻塞 I/O，是指应用程序执行 I/O 操作后，不会阻塞当前的线程，可以继续执行其他的任务，随后再通过轮询或者事件通知的形式，获取调用的结果
   
 - 根据**是否等待响应结果**，可以把文件 I/O 分为同步和异步 I/O
    - 同步 I/O，是指应用程序执行 I/O 操作后，要一直等到整个 I/O 完成后，才能获得 I/O 响应
    - 异步 I/O，是指应用程序执行 I/O 操作后，不用等待完成和完成后的响应，而是继续执行就可以。等到这次 I/O 完成后，响应会用事件通知的方式，告诉应用程序

### 性能观测

```
$ df -h /dev/sda1

$ df -i /dev/sda1
```

## [24 | 基础篇：Linux 磁盘I/O是怎么工作的（上）](https://time.geekbang.org/column/article/77010)

- 连续 I/O 还可以通过预读的方式，来减少 I/O 请求的次数，这也是其性能优异的一个原因

Linux 内核支持四种 I/O 调度算法

- NONE
- NOOP : 实际上是一个先入先出的队列，只做一些最基本的请求合并，常用于 SSD 磁盘
- CFQ
- DeadLine : 分别为读、写请求创建了不同的 I/O 队列，可以提高机械磁盘的吞吐量，并确保达到最终期限（deadline）的请求被优先处理。DeadLine 调度算法，多用在 I/O 压力比较重的场景，比如数据库等。

### I/O 栈

由上到下分为三个层次，分别是文件系统层、通用块层和设备层

- **文件系统层**，包括虚拟文件系统和其他各种文件系统的具体实现。它为上层的应用程序，提供标准的文件访问接口；对下会通过通用块层，来存储和管理磁盘数据。
- **通用块层**，包括块设备 I/O 队列和 I/O 调度器。它会对文件系统的 I/O 请求进行排队，再通过重新排序和请求合并，然后才要发送给下一级的设备层。
- **设备层**，包括存储设备和相应的驱动程序，负责最终物理设备的 I/O 操作。

存储系统的 I/O ，通常是整个系统中最慢的一环。所以， Linux 通过多种缓存机制来优化 I/O 效率。

## [25 | 基础篇：Linux 磁盘I/O是怎么工作的（下）](https://time.geekbang.org/column/article/77511)

### 磁盘性能指标

五个常见指标

- 使用率，是指磁盘处理 I/O 的时间百分比。过高的使用率（比如超过 80%），通常意味着磁盘 I/O 存在性能瓶颈。
    - 使用率只考虑有没有 I/O，而不考虑 I/O 的大小。换句话说，当使用率是 100% 的时候，磁盘依然有可能接受新的 I/O 请求
- 饱和度，是指磁盘处理 I/O 的繁忙程度。过高的饱和度，意味着磁盘存在严重的性能瓶颈。当饱和度为 100% 时，磁盘无法接受新的 I/O 请求。
- IOPS（Input/Output Per Second），是指每秒的 I/O 请求数。
- 吞吐量，是指每秒的 I/O 请求大小。
- 响应时间，是指 I/O 请求从发出到收到响应的间隔时间。

不要孤立地去比较某一指标，而要结合读写比例、I/O 类型（随机还是连续）以及 I/O 的大小，综合来分析

- 在数据库、大量小文件等这类随机读写比较多的场景中，IOPS 更能反映系统的整体性能；
- 而在多媒体等顺序读写较多的场景中，吞吐量才更能反映系统的整体性能。

性能测试工具 **fio** ，来测试磁盘的 IOPS、吞吐量以及响应时间等核心指标


```cmd
# -d -x表示显示所有磁盘I/O的指标
$ iostat -d -x 1
```
输出结果说明见原文插图

- **%util** ，就是我们前面提到的磁盘 I/O 使用率；
- **r/s+ w/s** ，就是 IOPS；
- **rkB/s+wkB/s** ，就是吞吐量；
- **r_await+w_await** ，就是响应时间。

观察进程的 I/O 情况，你还可以使用 pidstat 和 iotop 这两个工具。

```cmd
$ pidstat -d 1
```

iotop 可以按照 I/O 大小对进程排序，然后找到 I/O 较大的那些进程

```cmd
$ iotop
```

## [26 | 案例篇：如何找出狂打日志的“内鬼”？](https://time.geekbang.org/column/article/77885)

**lsof** 命令，看看进程都打开了哪些文件

```cmd
lsof -p 18940
```

## [27 | 案例篇：为什么我的磁盘I/O延迟很高？](https://time.geekbang.org/column/article/78409)

**filetop** 它是 bcc 软件包的一部分，基于 Linux 内核的 eBPF（extended Berkeley Packet Filters）机制，主要跟踪内核中文件的读写情况，并输出线程 ID（TID）、读写大小、读写类型以及文件名称。

```cmd
$ /snap/bin/bcc.filetop -C
```

**opensnoop** 它同属于 bcc 软件包，可以动态跟踪内核中的 open 系统调用

```cmd
$ /snap/bin/bcc.opensnoop
```

## [30 | 套路篇：如何迅速分析出系统I/O的瓶颈在哪里？](https://time.geekbang.org/column/article/79001)
套路直接看原文

## [31 | 套路篇：磁盘 I/O 性能优化的几个思路](https://time.geekbang.org/column/article/79368)

### I/O 基准测试

[fio](https://github.com/axboe/fio) （Flexible I/O Tester）

- 最常用的文件系统和磁盘 I/O 性能基准测试工具
- 提供了大量的可定制化选项，可以用来测试，裸盘或者文件系统在各种场景下的 I/O 性能，包括了不同块大小、不同 I/O 引擎以及是否使用缓存等场景。

通过 blktrace+fio 的组合使用，可以得到应用程序 I/O 模式的基准测试报告

## [32 | 答疑（四）：阻塞、非阻塞 I/O 与同步、异步 I/O 的区别和联系](https://time.geekbang.org/column/article/79734)

阻塞 / 非阻塞和同步 / 异步，其实就是两个不同角度的 I/O 划分方式。它们描述的对象也不同

- 阻塞 / 非阻塞针对的是 I/O **调用者**（即应用程序）
- 同步 / 异步针对的是 I/O **执行者**（即系统）

## [34 | 关于 Linux 网络，你必须知道这些（下）](https://time.geekbang.org/column/article/81057)

### 性能指标

- **带宽**，表示链路的最大传输速率，单位通常为 b/s （比特 / 秒）。
- **吞吐量**，表示单位时间内成功传输的数据量，单位通常为 b/s（比特 / 秒）或者 B/s（字节 / 秒）。吞吐量受带宽限制，而吞吐量 / 带宽，也就是该网络的使用率。
- **延时**，表示从网络请求发出后，一直到收到远端响应，所需要的时间延迟。在不同场景中，这一指标可能会有不同含义。比如，它可以表示，建立连接需要的时间（比如 TCP 握手延时），或一个数据包往返所需的时间（比如 RTT）。
- **PPS**，是 Packet Per Second（包 / 秒）的缩写，表示以网络包为单位的传输速率。PPS 通常用来评估网络的转发能力，比如硬件交换机，通常可以达到线性转发（即 PPS 可以达到或者接近理论最大值）。而基于 Linux 服务器的转发，则容易受网络包大小的影响。
- 除了这些指标，**网络的可用性**（网络能否正常通信）、**并发连接数**（TCP 连接数量）、**丢包率**（丢包百分比）、**重传率**（重新传输的网络包比例）等也是常用的性能指标。

### 网络配置

可以使用 ifconfig 或者 ip 命令，来查看网络的配置

 - ifconfig 和 ip **只显示了网络接口收发数据包的统计信息**
 - ip 工具提供了更丰富的功能和更易用的接口

 以网络接口 eth0 为例，你可以运行下面的两个命令，查看它的配置和状态：
 
 ```cmd
 $ ifconfig eth0
 
 $ ip -s addr show dev eth0
 ```

#### 1. 网络接口的状态标志
表示物理网络是连通的，即网卡已经连接到了交换机或者路由器中

- ifconfig 输出中的 RUNNING 
- ip 输出中的 LOWER_UP

#### 2. MTU 的大小
MTU 默认大小是 1500，根据网络架构的不同（比如是否使用了 VXLAN 等叠加网络），你可能需要调大或者调小 MTU 的数值。

#### 3. 网络接口的 IP 地址、子网以及 MAC 地址
这些都是保障网络功能正常工作所必需的，需要确保配置正确。

#### 4. 网络收发的字节数、包数、错误数以及丢包情况
特别是 TX 和 RX 部分的 errors、dropped、overruns、carrier 以及 collisions 等指标不为 0 时，通常表示出现了网络 I/O 问题。

- **errors** 表示发生错误的数据包数，比如校验错误、帧同步错误等；

- **dropped** 表示丢弃的数据包数，即数据包已经收到了 Ring Buffer，但因为内存不足等原因丢包；
- **overruns** 表示超限数据包数，即网络 I/O 速度过快，导致 Ring Buffer 中的数据包来不及处理（队列满）而导致的丢包；
- **carrier** 表示发生 carrirer 错误的数据包数，比如双工模式不匹配、物理电缆出现问题等；collisions 表示碰撞数据包数。

### 套接字信息

网络协议栈中的统计信息，可以用 netstat 或者 ss ，来查看套接字、网络栈、网络接口以及路由表的信息。

推荐使用 ss 来查询网络的连接信息，因为它比 netstat 提供了更好的性能（速度更快）。

```cmd
# head -n 3 表示只显示前面3行
# -l 表示只显示监听套接字
# -n 表示显示数字地址和端口(而不是名字)
# -p 表示显示进程信息
$ netstat -nlp | head -n 3

# -l 表示只显示监听套接字
# -t 表示只显示 TCP 套接字
# -n 表示显示数字地址和端口(而不是名字)
# -p 表示显示进程信息
$ ss -ltnp | head -n 3
```

- netstat 和 ss 的输出也是类似的，都展示了套接字的状态、接收队列、发送队列、本地地址、远端地址、进程 PID 和进程名称等。

- 接收队列（Recv-Q）和发送队列（Send-Q）需要你特别关注，它们通常应该是 0。当你发现它们不是 0 时，说明有网络包的堆积发生。当然还要注意，在不同套接字状态下，它们的含义不同。
    - 当套接字处于连接状态（Established）时
        - Recv-Q 表示套接字缓冲还没有被应用程序取走的字节数（即接收队列长度）。
        - Send-Q 表示还没有被远端主机确认的字节数（即发送队列长度）。
    
    - 当套接字处于监听状态（Listening）时
        - Recv-Q 表示**全连接**队列的长度。
        - Send-Q 表示**全连接**队列的最大长度。

            - 全连接，是指服务器收到了客户端的 ACK，完成了 TCP 三次握手，然后就会把这个连接挪到全连接队列中。这些全连接中的套接字，还需要被 accept() 系统调用取走，服务器才可以开始真正处理客户端的请求。与全连接队列相对应的，还有一个半连接队列。

            - 半连接是指还没有完成 TCP 三次握手的连接，连接只进行了一半。服务器收到了客户端的 SYN 包后，就会把这个连接放到半连接队列中，然后再向客户端发送 SYN+ACK 包。

### 协议栈统计信息

使用 netstat 或 ss ，也可以查看协议栈的信息

```cmd
$ netstat -s

$ ss -s
```

ss 只显示已经连接、关闭、孤儿套接字等简要统计，而 netstat 则提供的是更详细的网络协议栈信息。

### 网络吞吐和 PPS

- 推荐使用 sar

- 给 sar 增加 -n 参数就可以查看网络的统计信息，比如网络接口（DEV）、网络接口错误（EDEV）、TCP、UDP、ICMP 等等。执行下面的命令，你就可以得到网络接口统计信息：

```cmd
# 数字1表示每隔1秒输出一组数据
$ sar -n DEV 1
```

- **rxpck/s 和 txpck/s** 分别是接收和发送的 PPS，单位为包 / 秒。
- **rxkB/s 和 txkB/s** 分别是接收和发送的吞吐量，单位是 KB/ 秒。
- **rxcmp/s 和 txcmp/s** 分别是接收和发送的压缩数据包数，单位是包 / 秒。
- **%ifutil** 是网络接口的使用率，即半双工模式下为 (rxkB/s+txkB/s)/Bandwidth，而全双工模式下为 max(rxkB/s, txkB/s)/Bandwidth。

#### 查看网卡速度

```cmd
$ ethtool eth0 | grep Speed
```

### 连通性和延时

使用 ping ，来测试远程主机的连通性和延时，而这基于 ICMP 协议

```cmd
# -c3表示发送三次ICMP包后停止
$ ping -c3 114.114.114.114
```

ping 的输出，可以分为两部分。

- 第一部分，是每个 ICMP 请求的信息，包括 ICMP 序列号（icmp_seq）、TTL（生存时间，或者跳数）以及往返延时。
- 第二部分，则是三次 ICMP 请求的汇总。

## [35 | 基础篇：C10K 和 C1000K 回顾](https://time.geekbang.org/column/article/81268)

### I/O 模型优化

I/O 多路复用（I/O Multiplexing）

#### 第一种，使用非阻塞 I/O 和水平触发通知，比如使用 select 或者 poll

- 最大优点，是对应用程序比较友好，它的 API 非常简单。
- select 和 poll 还有一些其他的限制
    - select 轮询时间复杂度 O(n^2)
    - poll 轮询时间复杂度 O(n)
    - 内核空间与用户空间切换，增加了处理成本

#### 第二种，使用非阻塞 I/O 和边缘触发通知，比如 epoll

- epoll 使用红黑树，在内核中管理文件描述符的集合，这样，就不需要应用程序在每次操作时都传入、传出这个集合。
- epoll 使用事件驱动的机制，只关注有 I/O 事件发生的文件描述符，不需要轮询扫描整个集合。

#### 第三种，使用异步 I/O（Asynchronous I/O，简称为 AIO）
- 由于异步 I/O 跟我们的直观逻辑不太一样，想要使用的话，一定要小心设计，其使用难度比较高。

### 工作模型优化

- 第一种，主进程 + 多个 worker 子进程，这也是最常用的一种模型。
    - 例如 Nginx
    - 为了避免惊群问题， Nginx 在每个 worker 进程中，都增加一个了全局锁（accept_mutex）。

- 第二种，监听到相同端口的多进程模型。
    - 由于内核确保了只有一个进程被唤醒，就不会出现惊群问题
    - Nginx 在 1.9.1 中就已经支持了这种模式

### 小结

- 从 C10K 到 C100K ，可能只需要增加系统的物理资源就可以满足；
- 从 C100K 到 C1000K ，就不仅仅是增加物理资源就能解决的问题了。
- 实现 C10M 
    - 需要用 XDP 的方式，在内核协议栈之前处理网络包；
    - 或者用 DPDK 直接跳过网络协议栈，在用户空间通过轮询的方式直接处理网络包。

## [36 | 套路篇：怎么评估系统的网络性能？](https://time.geekbang.org/column/article/81497)

### 各协议层的性能测试

#### 转发性能

- hping3 测试网络包处理能力的性能工具
- [pktgen](https://wiki.linuxfoundation.org/networking/pktgen) Linux 内核自带的高性能网络测试工具

```cmd
$ modprobe pktgen
$ ps -ef | grep pktgen | grep -v grep
root     26384     2  0 06:17 ?        00:00:00 [kpktgend_0]
root     26385     2  0 06:17 ?        00:00:00 [kpktgend_1]
$ ls /proc/net/pktgen/
kpktgend_0  kpktgend_1  pgctrl
```

#### TCP/UDP 性能

iperf 和 netperf 都是最常用的网络性能测试工具，测试 TCP 和 UDP 的吞吐量。它们都以客户端和服务器通信的方式，测试一段时间内的平均吞吐量。

##### iperf

```cmd
$ apt-get install iperf3
```

需要2台机器进行测试：客户端、服务端

#### HTTP 性能

ab、webbench 等，都是常用的 HTTP 压力测试工具。其中，ab 是 Apache 自带的 HTTP 压测工具，主要测试 HTTP 服务的每秒请求数、请求延迟、吞吐量以及请求延迟的分布情况等。

#### 应用负载性能

wrk、TCPCopy、Jmeter 或者 LoadRunner

## [37 | 案例篇：DNS 解析时快时慢，我该怎么办？](https://time.geekbang.org/column/article/81850)

- 在应用层，我们关注的是应用程序的并发连接数、每秒请求数、处理延迟、错误数等，可以使用 wrk、JMeter 等工具，模拟用户的负载，得到想要的测试结果。

- 在传输层，我们关注的是 TCP、UDP 等传输层协议的工作状况，比如 TCP 连接数、 TCP 重传、TCP 错误数等。此时，你可以使用 iperf、netperf 等，来测试 TCP 或 UDP 的性能。
- 再向下到网络层，我们关注的则是网络包的处理能力，即 PPS。Linux 内核自带的 pktgen，就可以帮你测试这个指标。
- 由于低层协议是高层协议的基础，所以一般情况下，我们所说的网络优化，实际上包含了整个网络协议栈的所有层的优化。当然，性能要求不同，具体需要优化的位置和目标并不完全相同。


以极客时间的网站 time.geekbang.org 为例，执行下面的 nslookup 命令，就可以查询到这个域名的 A 记录，可以看到，它的 IP 地址是 39.106.233.176：

```cmd
$ nslookup time.geekbang.org
# 域名服务器及端口信息
Server:    114.114.114.114
Address:  114.114.114.114#53

# 非权威查询结果
Non-authoritative answer:
Name:  time.geekbang.org
Address: 39.106.233.17
```

常用的 DNS 解析工具 **dig** ，就提供了 trace 功能，可以展示递归查询的整个过程

```cmd
# +trace表示开启跟踪查询
# +nodnssec表示禁止DNS安全扩展
$ dig +trace +nodnssec www.aoeai.com
```

dig trace 的输出，主要包括四部分。

- 第一部分，是从 114.114.114.114 查到的一些根域名服务器（.）的 NS 记录。
- 第二部分，是从 NS 记录结果中选一个（h.root-servers.net），并查询顶级域名 org. 的 NS 记录。
- 第三部分，是从 org. 的 NS 记录中选择一个（b0.org.afilias-nst.org），并查询二级域名 geekbang.org. 的 NS 服务器。
- 最后一部分，就是从 geekbang.org. 的 NS 服务器（dns10.hichina.com）查询最终主机 time.geekbang.org. 的 A 记录。

**dnsmasq** 是最常用的 DNS 缓存服务之一，还经常作为 DHCP 服务来使用。它的安装和配置都比较简单，性能也可以满足绝大多数应用程序对 DNS 缓存的需求。

### 小结
- 使用 **HTTPDNS** 取代常规的 DNS 解析。这是很多移动应用会选择的方法，特别是如今域名劫持普遍存在，使用 HTTP 协议绕过链路中的 DNS 服务器，就可以避免域名劫持的问题。
- 基于 DNS 的全局负载均衡（GSLB）。这不仅为服务提供了负载均衡和高可用的功能，还可以根据用户的位置，返回距离最近的 IP 地址。

## [38 | 案例篇：怎么使用 tcpdump 和 Wireshark 分析网络流量？](https://time.geekbang.org/column/article/82321)

tcpdump 和 [Wireshark](https://www.wireshark.org/) 就是最常用的网络抓包和分析工具，更是分析网络性能必不可少的利器。

- tcpdump 仅支持命令行格式使用，常用在服务器中抓取和分析网络包。
- Wireshark 除了可以抓包外，还提供了强大的图形界面和汇总分析工具，在分析复杂的网络情景时，尤为简单和实用。
- 在实际分析网络性能时，先用 tcpdump 抓包，后用 Wireshark 分析，也是一种常用的方法。

```cmd
$ apt-get install tcpdump wireshark
```

tcpdump 使用见原文插图

执行下面的命令，把抓取的网络包保存到 ping.pcap 文件中：

```cmd
$ tcpdump -nn udp port 53 or host 35.190.27.188 -w ping.pcap
```

用 scp 把它拷贝到本地来

```cmd
scp host-ip/path/ping.pcap .
```

然后，再用 **Wireshark** 打开它

wireshark 的使用推荐阅读林沛满的《Wireshark网络分析就这么简单》和《Wireshark网络分析的艺术》

## [40 | 案例篇：网络请求延迟变大了，我该怎么办？](https://time.geekbang.org/column/article/82833)

- ping 基于 **ICMP 协议**，它通过计算 ICMP 回显响应报文与 ICMP 回显请求报文的时间差，来获得往返延时。

- 很多网络服务会把 ICMP 禁止掉，这也就导致我们无法用 ping ，来测试网络服务的可用性和往返延时。这时，你可以用 **traceroute** 或 **hping3** 的 TCP 和 UDP 模式，来获取网络延迟。

以 baidu.com 为例，你可以执行下面的 hping3 命令，测试你的机器到百度搜索服务器的网络延迟：

```cmd
# -c表示发送3次请求，-S表示设置TCP SYN，-p表示端口号为80
$ hping3 -c 3 -S -p 80 baidu.com
```

用 traceroute ，也可以得到类似结果

```cmd
# --tcp表示使用TCP协议，-p表示端口号，-n表示不对结果中的IP地址执行反向域名解析
$ traceroute --tcp -p 80 -n baidu.com
```

## [41 | 案例篇：如何优化 NAT 性能？（上）](https://time.geekbang.org/column/article/83189)

另一个可能导致网络延迟的因素，即网络地址转换（Network Address Translation），缩写为 NAT

## [42 | 案例篇：如何优化 NAT 性能？（下）](https://time.geekbang.org/column/article/83520)

[SystemTap](https://sourceware.org/systemtap/) 是 Linux 的一种动态追踪框架，它把用户提供的脚本，转换为内核模块来执行，用来监测和跟踪内核的行为。

## [43 | 套路篇：网络性能优化的几个思路（上）](https://time.geekbang.org/column/article/83783)

### 为了提高网络的吞吐量，你通常需要调整这些缓冲区的大小

- 增大每个套接字的缓冲区大小 net.core.optmem_max；
- 增大套接字接收缓冲区大小 net.core.rmem_max 和发送缓冲区大小 net.core.wmem_max；
- 增大 TCP 接收缓冲区大小 net.ipv4.tcp_rmem 和发送缓冲区大小 net.ipv4.tcp_wmem。
- 更多见图

### 除此之外，套接字接口还提供了一些配置选项，用来修改网络连接的行为：
- 为 TCP 连接设置 TCP_NODELAY 后，就可以禁用 Nagle 算法；
- 为 TCP 连接开启 TCP_CORK 后，可以让小包聚合成大包后再发送（注意会阻塞小包的发送）；
- 使用 SO_SNDBUF 和 SO_RCVBUF ，可以分别调整套接字发送缓冲区和接收缓冲区的大小。

## [44 | 套路篇：网络性能优化的几个思路（下）](https://time.geekbang.org/column/article/84003)

### 网络性能优化

#### 传输层

- 传输层最重要的是 TCP 和 UDP 协议，所以这儿的优化，其实主要就是对这两种协议的优化。

##### TCP 协议的优化

- 第一类，在请求数比较大的场景下，你可能会看到大量处于 TIME_WAIT 状态的连接，它们会占用大量内存和端口资源。这时，我们可以优化与 TIME_WAIT 状态相关的内核选项，比如采取下面几种措施。
    - 增大处于 TIME_WAIT 状态的连接数量 net.ipv4.tcp_max_tw_buckets ，并增大连接跟踪表的大小 net.netfilter.nf_conntrack_max。
    - 减小 net.ipv4.tcp_fin_timeout 和 net.netfilter.nf_conntrack_tcp_timeout_time_wait ，让系统尽快释放它们所占用的资源。
    - 开启端口复用 net.ipv4.tcp_tw_reuse。这样，被 TIME_WAIT 状态占用的端口，还能用到新建的连接中。
    - 增大本地端口的范围 net.ipv4.ip_local_port_range 。这样就可以支持更多连接，提高整体的并发能力。
    - 增加最大文件描述符的数量。你可以使用 fs.nr_open 和 fs.file-max ，分别增大进程和系统的最大文件描述符数；或在应用程序的 systemd 配置文件中，配置 LimitNOFILE ，设置应用程序的最大文件描述符数。

- 第二类，为了缓解 SYN FLOOD 等，利用 TCP 协议特点进行攻击而引发的性能问题，你可以考虑优化与 SYN 状态相关的内核选项
- 第三类，在长连接的场景中，通常使用 Keepalive 来检测 TCP 连接的状态，以便对端连接断开后，可以自动回收。但是，系统默认的 Keepalive 探测间隔和重试次数，一般都无法满足应用程序的性能要求。所以，这时候你需要优化与 Keepalive 相关的内核选项

 **优化 TCP 性能时，你还要注意，如果同时使用不同优化方法，可能会产生冲突**

- 网络请求延迟的案例中我们曾经分析过的，服务器端开启 Nagle 算法，而客户端开启延迟确认机制，就很容易导致网络延迟增大。
- 在使用 NAT 的服务器上，如果开启 net.ipv4.tcp_tw_recycle ，就很容易导致各种连接失败。实际上，由于坑太多，这个选项在内核的 4.1 版本中已经删除了。

##### UDP 的优化
- 跟上篇套接字部分提到的一样，增大套接字缓冲区大小以及 UDP 缓冲区范围；
- 跟前面 TCP 部分提到的一样，增大本地端口号的范围；
- 根据 MTU 大小，调整 UDP 数据包的大小，减少或者避免分片的发生。

#### 网络层

网络层，负责网络包的封装、寻址和路由，包括 IP、ICMP 等常见协议。在网络层，最主要的优化，其实就是对路由、 IP 分片以及 ICMP 等进行调优。

##### 第一种，从路由和转发的角度出发，你可以调整下面的内核选项
- 在需要转发的服务器中，比如用作 NAT 网关的服务器或者使用 Docker 容器时，开启 IP 转发，即设置 net.ipv4.ip_forward = 1。

- 调整数据包的生存周期 TTL，比如设置 net.ipv4.ip_default_ttl = 64。注意，增大该值会降低系统性能。
- 开启数据包的反向地址校验，比如设置 net.ipv4.conf.eth0.rp_filter = 1。这样可以防止 IP 欺骗，并减少伪造 IP 带来的 DDoS 问题。

##### 第二种，从分片的角度出发，最主要的是调整 MTU（Maximum Transmission Unit）的大小。

##### 第三种，从 ICMP 的角度出发，为了避免 ICMP 主机探测、ICMP Flood 等各种网络问题，你可以通过内核选项，来限制 ICMP 的行为。

- 可以禁止 ICMP 协议，即设置 net.ipv4.icmp_echo_ignore_all = 1。这样，外部主机就无法通过 ICMP 来探测主机。

- 可以禁止广播 ICMP，即设置 net.ipv4.icmp_echo_ignore_broadcasts = 1。

#### 链路层

链路层负责网络包在物理网络中的传输，比如 MAC 寻址、错误侦测以及通过网卡传输网络帧等。自然，链路层的优化，也是围绕这些基本功能进行的。

##### 由于网卡收包后调用的中断处理程序（特别是软中断），需要消耗大量的 CPU。所以，将这些中断处理程序调度到不同的 CPU 上执行，就可以显著提高网络吞吐量。这通常可以采用下面两种方法。

- 可以为网卡硬中断配置 CPU 亲和性（smp_affinity），或者开启 irqbalance 服务。
- 可以开启 RPS（Receive Packet Steering）和 RFS（Receive Flow Steering），将应用程序和软中断的处理，调度到相同 CPU 上，这样就可以增加 CPU 缓存命中率，减少网络延迟。

##### 现在的网卡都有很丰富的功能，原来在内核中通过软件处理的功能，可以卸载到网卡中，通过硬件来执行。
- **TSO**（TCP Segmentation Offload）和 UFO（UDP Fragmentation Offload）：在 TCP/UDP 协议中直接发送大包；而 TCP 包的分段（按照 MSS 分段）和 UDP 的分片（按照 MTU 分片）功能，由网卡来完成 。

- **GSO**（Generic Segmentation Offload）：在网卡不支持 TSO/UFO 时，将 TCP/UDP 包的分段，延迟到进入网卡前再执行。这样，不仅可以减少 CPU 的消耗，还可以在发生丢包时只重传分段后的包。
- **LRO**（Large Receive Offload）：在接收 TCP 分段包时，由网卡将其组装合并后，再交给上层网络处理。不过要注意，在需要 IP 转发的情况下，不能开启 LRO，因为如果多个包的头部信息不一致，LRO 合并会导致网络包的校验错误。
- **GRO**（Generic Receive Offload）：GRO 修复了 LRO 的缺陷，并且更为通用，同时支持 TCP 和 UDP。RSS（Receive Side Scaling）：也称为多队列接收，它基于硬件的多个接收队列，来分配网络接收进程，这样可以让多个 CPU 来处理接收到的网络包。
- **VXLAN** 卸载：也就是让网卡来完成 VXLAN 的组包功能。

##### 对于网络接口本身，也有很多方法，可以优化网络的吞吐量
- 可以开启网络接口的多队列功能。这样，每个队列就可以用不同的中断号，调度到不同 CPU 上执行，从而提升网络的吞吐量。

- 可以增大网络接口的缓冲区大小，以及队列长度等，提升网络传输的吞吐量（注意，这可能导致延迟增大）。
- 可以使用 Traffic Control 工具，为不同网络流量配置 QoS。

##### C10M
- DPDK
- XDP

### 小结

- 在应用程序中，主要是优化 I/O 模型、工作模型以及应用层的网络协议；

- 在套接字层中，主要是优化套接字的缓冲区大小；
- 在传输层中，主要是优化 TCP 和 UDP 协议；
- 在网络层中，主要是优化路由、转发、分片以及 ICMP 协议；最后，在链路层中，主要是优化网络包的收发、网络功能卸载以及网卡选项。

## [49 | 案例篇：内核线程 CPU 利用率太高，我该怎么办？](https://time.geekbang.org/column/article/86330)

### 火焰图

针对 perf 汇总数据的展示问题，Brendan Gragg 发明了[火焰图](http://www.brendangregg.com/flamegraphs.html)，通过矢量图的形式，更直观展示汇总结果。

- **横轴表示采样数和采样比例**。一个函数占用的横轴越宽，就代表它的执行时间越长。同一层的多个函数，则是按照字母来排序。

- **纵轴表示调用栈**，由下往上根据调用关系逐个展开。换句话说，上下相邻的两个函数中，下面的函数，是上面函数的父函数。这样，调用栈越深，纵轴就越高。
- 另外，要注意图中的颜色，并没有特殊含义，只是用来区分不同的函数。

## [50 | 案例篇：动态追踪怎么用？（上）](https://time.geekbang.org/column/article/86490)

使用 perf 对系统内核线程进行分析时，内核线程依然还在正常运行中，所以这种方法也被称为动态追踪技术。

**动态追踪技术，通过探针机制，来采集内核或者应用程序的运行信息，从而可以不用修改内核和应用程序的代码，就获得丰富的信息，帮你分析、定位想要排查的问题。**

相比以往的进程级跟踪方法（比如 ptrace），动态追踪往往只会带来很小的性能损耗（通常在 5% 或者更少）。

### 动态追踪

常见的动态追踪方法包括 ftrace、perf、eBPF 以及 SystemTap

#### ftrace

- 当你已经定位了某个内核函数，但不清楚它的实现原理时，就可以用 ftrace 来跟踪它的执行过程。

- 提供了多个跟踪器，用于跟踪不同类型的信息，比如函数调用、中断关闭、进程调度等。具体支持的跟踪器取决于系统配置。

```cmd
$ apt-get install trace-cmd
```

## [51 | 案例篇：动态追踪怎么用？（下）](https://time.geekbang.org/column/article/86710)

### perf
- 查找应用程序或者内核中的热点函数，从而定位性能瓶颈

- 使用火焰图动态展示 perf 的事件记录，从而更直观地发现了问题
- perf 可以用来分析 CPU cache、CPU 迁移、分支预测、指令周期等各种硬件事件；
- perf 也可以只对感兴趣的事件进行动态追踪。

同 ftrace 一样，你也可以通过 perf list ，查询所有支持的事件：

```cmd
$ perf list
```

很多人只看到了 strace 简单易用的好处，却忽略了它对进程性能带来的影响。从原理上来说，**strace 基于系统调用 ptrace 实现**，这就带来了两个问题。

- 由于 ptrace 是系统调用，就需要在内核态和用户态切换。当事件数量比较多时，繁忙的切换必然会影响原有服务的性能；
- ptrace 需要借助 SIGSTOP 信号挂起目标进程。这种信号控制和进程挂起，会影响目标进程的行为。

在性能敏感的应用（比如数据库）中，不推荐你用 **strace** （或者其他**基于 ptrace 的性能工具**）去排查和调试。

### eBPF 和 BCC

ftrace 和 perf 的功能已经比较丰富了，不过，它们有一个共同的缺陷，那就是不够灵活，没法像 DTrace 那样通过脚本自由扩展。

### SystemTap 和 sysdig
- SystemTap 只在 RHEL 系统中好用，在其他系统中则容易出现各种异常问题

- sysdig 则是随着容器技术的普及而诞生的，主要用于容器的动态追踪。
- sysdig 汇集了一些列性能工具的优势
- sysdig = strace + tcpdump + htop + iftop + lsof + docker inspect
- 在最新的版本中（内核版本 >= 4.14），sysdig 还可以通过 eBPF 来进行扩展，所以，也可以用来追踪内核中的各种函数和事件。

### 如何选择追踪工具
见原文插图

- 在新版的内核中，eBPF 和 BCC 是最灵活的动态追踪方法

## [53 | 套路篇：系统监控的综合思路](https://time.geekbang.org/column/article/87980)

### USE 法
一种专门用于性能监控的 USE（Utilization Saturation and Errors）法。USE 法把系统资源的性能指标，简化成了三个类别，即使用率、饱和度以及错误数。

- 使用率，表示资源用于服务的时间或容量百分比。100% 的使用率，表示容量已经用尽或者全部时间都用于服务。

- 饱和度，表示资源的繁忙程度，通常与等待队列的长度相关。100% 的饱和度，表示资源无法接受更多的请求。
- 错误数表示发生错误的事件个数。错误数越多，表明系统的问题越严重。

无论是对 CPU、内存、磁盘和文件系统、网络等硬件资源，还是对文件描述符数、连接数、连接跟踪数等软件资源，USE 方法都可以帮你快速定位出，是哪一种系统资源出现了性能瓶颈。

### 监控系统

常见开源的监控工具：Zabbix、Nagios、Prometheus

## [54 | 套路篇：应用监控的一般思路](https://time.geekbang.org/column/article/88423)

### RED原则 
RED方法更偏重于应用

- Rate (R): The number of requests per second.
- Errors (E): The number of failed requests.
- Duration (D): The amount of time to process a request.

### 指标监控
- 请求数、错误率和响应时间
- 可以使用 Zipkin、Jaeger、Pinpoint 等各类开源工具，来构建全链路跟踪系统。

### 日志监控
对日志监控来说，最经典的方法，就是使用 ELK 技术栈

## [55 | 套路篇：分析性能问题的一般步骤](https://time.geekbang.org/column/article/88667)
套路满满见原文

## [56 | 套路篇：优化性能问题的一般方法](https://time.geekbang.org/column/article/89278)
套路满满见原文

## [57 | 套路篇：Linux 性能工具速查](https://time.geekbang.org/column/article/89306)
见原文插图

## [加餐（一） | 书单推荐：性能优化和Linux 系统原理](https://time.geekbang.org/column/article/80829)
- Linux 基础入门书籍：《鸟哥的 Linux 私房菜》
- 计算机原理书籍：《深入理解计算机系统》
- Linux 编程书籍：《Linux 程序设计》和《UNIX 环境高级编程》
- Linux 内核书籍：《深入 Linux 内核架构》
- 性能优化书籍：《性能之巅：洞悉系统、企业与云计算》

## [加餐（二） | 书单推荐：网络原理和 Linux 内核实现](https://time.geekbang.org/column/article/84619)
- 计算机网络经典教材《计算机网络（第 5 版）》
- 网络协议必读书籍《TCP/IP 详解 卷 1：协议》
- Wireshark 书籍《Wireshark 网络分析就这么简单》和《Wireshark 网络分析的艺术》
- 网络编程书籍《UNIX 网络编程》



