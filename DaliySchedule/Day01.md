# Day01

2022年9月1日 第一天

我大概有点小基础（其实很水👀️ ），就直接去做小练习了

### 配置Github Classroom模式的Rustling小练习

首先接受邀请 [Rust-lang Lab Test based on Rustlings](https://classroom.github.com/a/YTNg1dEH)

在生成的github链接上，找到code，也就是平时我们经常去git clone的那个链接的部分，不过这次有特殊的选项，就是 `codespace` ，如下图所示

![day01_00](/photos/day01_00.png)

但是在 `sudo make codespaces_setenv`  后并没有正常执行完全，
大概是这个样子:
`To get started you may need to restart your current shell.`
`This would reload your PATH environment variable to include`
`Cargo's bin directory ($HOME/.cargo/bin).`

`To configure your current shell, run:`
`source "$HOME/.cargo/env"`
`/bin/zsh && source /home/codespace/.cargo/env`

需手动在终端输入
`source "$HOME/.cargo/env" /bin/zsh && source /home/codespace/.cargo/env`
以及
`cargo install --force --path .`
此时再输入 `rustlings` 即可出现测验信息。

### 使用方法

输入 `rustlings watch` 将会显示通过测试的练习，如图示

![day01_01](/photos/day01_01.png)

删除注释里面的 `I AM NOT DONE` 则第一个练习通过

![day01_02](/photos/day01_02.png)

如若获取提示，可以新建一个终端
再执行 `rustlings hint ***`
如 `rustlings hint functions1`

![day01_03](/photos/day01_03.png)

提示 Add an argument after the format string.

- 注：  

如果长时间无操作的话，会断开连接，重新建立连接，需重新执行操作

不过断开连接后，我在普通用户下，执行了`cargo install --force --path .`   
也是可以的


结束后，输入下列命令   
`git add -A`    
`git commit -a`  
在git commit文件中写入commit信息，保存，   也可以执行一下test   
`make test`  
看看通过的测试

![day01_05](/photos/day01_05.png)

### 其余进度

- [x] 完成3个exercises
- [x] rust圣经阅读到 流程控制 以及做了部分课后练习，没全做完，感觉有点多

| Exercise  |
|-----------|
| variables |
| functions |
| if        | 
| quiz1     |

![day01_04](/photos/day01_04.png)

### 收获

语句和表达式那边绕了，主要是在一个函数返回时，如过是用了return，加不加 `；` 都无所谓，
不用return的话，即用表达式或者语句返回，此时，语句即加了 `;` 的表达式以及 赋值表达式 如 `x += 1` 这种 ,返回的都是`()`，
可以做做rust圣经对应的练习和看看评论区

if2 很有趣  
 
```
note:`if` expressions without `else` evaluate to `()`
```

### 参考资料

[rust圣经](https://course.rs/about-book.html)   
[Rust by practice](https://zh.practice.rs/why-exercise.html)



