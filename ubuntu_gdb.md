# gdb

1. GDB功能及命令
命令形式 | 功能解释 | 示例(gdb)
--- | --- | ---
gdb | 进入gdb调试 | gdb
help | 显示帮助信息 | help
quit | 退出GDB调试|q (quit)
fiel <filename> | 加载被高度的可执行程序文件，在编译时要加上`-g`选项 | file test_gdb
list | 列出文件内容 | l (list)
run | 运行高度的程序（若有断点，会在断点处停止）| r (run)
break <function name> | 在某个函数调用处设断点 | b get_sum
break <line number> | 在某行设断点 | b (break) 24
break <line number> if condition | 在某行设置条件断点 | b 23 if index==3
delete <break number> | 删除断点编号对应的断点 | d (delete) 1
clear | 清空所有的断点信息 | clear
continue | 继续执行程序直到下一个断点或程序结束 | c (continue)
next | 单步调试 | n (next)
step | 遇到函数调用时，进入函数内部高度 | s (step)
print <value> | 显示变量的值 | p (print) index
info <> | 用来显示各类信息，详情查看“help info” | i (info) break
