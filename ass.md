// 1. 汇编指令
// 2. 寄存器

// 硬盘（程序）-> 内存 -> CPU
// CPU: 寄存器（信息存储） + 运算器（信息处理） + 控制器（控制其他器件进行工作）

// 64bit
// RAX\RBX\RCX\RDX 通用寄存器（常见的） 8个字节

//  |   |EAX| (RAX) 64bit
//		 EAX -> EAX 32bit	|  |AX|
//								AX -> |AH|AL|

// 32bit 
// EAX\EBX\ECX\EDX 通用寄存器（常见的） 4个字节

// 16bit	
// AX\BX\CX\DX	2个字节 

// mov dest, src
// 将src的内容赋值给dest
// [address] [地址值]
// mov dword ptr [1111h], 3	// 将3放入某个内存地址
// mov eax, dword ptr [1122H]
// word 代表2个字节 
// dword 代表4个字节(double word)
// qword 代表8个字节(quad word)
// 4个字节存储3


// 00 00 00 03H (16进制）
//  高字节放高地址（小端模式）
//如：112BH	   112CH	112DH	112EH
// 00000000	00000000 00000000 00000011 （2进制）
// CPU大小端模式，小端模式从高地址读，大部分都是小端模式
// 调试->窗口->内存 （可查看变量在内存的存储情况，了解内存存放数据的大小端模式）


// call 函数地址 -> 函数调用

// lea dest, [地址值] -> 把地址址给dest,类似于 dest = 地址值
// lea eax, [1122H]	-> eax == 1122H
// mov eax, dword ptr [1122H]

// ptr 
// ret 函数返回 return
// xor op1, op2 异或，将op1和op2异或的结果赋值给op1，类似于：op1 = op1 ^ op2
// add op1, op2 加法,类似于 op1 = op1 + op2
// sub op1, op2	减法，类似于 op1 = op1 - op2
// inc op	自增 increase，类似于 op = op + 1
// dec op	自减 decrease
// jmp 内存地址	跳到相应的地址去执行代码，j开头的一般都是跳转，大多数是带条件的跳转，一般跟test、cmp等

// cmp 比较两个值 compare
// jne jump not equal
