# 用户态程序

`user/hello_world.c` 是一个使用 ChCore libc 的用户态程序。它编译成 `ramdisk/hello_world.bin` 后随 ramdisk 打入镜像。系统启动时会运行这个程序，评分器通过它的终端输出检查用户态程序是否成功运行。

```text
Hello ChCore!
```

> [!HINT]
>
> - ChCore 的编译工具链在 `build/chcore-libc/bin` 文件夹中。
> - 如使用 cmake 进行编译，可以将工具链文件指定为 `build/toolchain.cmake`，将默认使用 ChCore 编译工具链。

到这里，你的程序应该可以通过所有的测试点并且获得满分。你可以编写一些更复杂的程序并尝试放入 ChCore 中运行。
