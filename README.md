# 第1章
### 检测点1.1
- 13 &emsp; 15 &emsp; 78 &emsp; 255 &emsp; 128 &emsp; 56091
### 检测点1.2
- 1000 &emsp; 1010 &emsp; 1100 &emsp; 1111 &emsp; 11001 &emsp; 100,0000 &emsp; 110,0100  
1111,1111,1111,1111 &emsp; 1,0000,0000,0000,0000,0000
### 检测点1.3
- 8 &emsp; 10 &emsp; 11 &emsp; 12 &emsp; 13 &emsp; 14 &emsp; 15 &emsp; 16 &emsp; 31 &emsp; 1741 &emsp; 1022 &emsp; 4092 &emsp; 65535
### 检测点1.4
- 8 &emsp; A &emsp; C &emsp; F &emsp; 19 &emsp; 40 &emsp; 64 &emsp; FF &emsp; 3E8 &emsp; FFFF &emsp; 10,0000
### 检测点1.5
1. 将下列十六进制数转换成二进制数  
11 &emsp; 1010 &emsp; 1100 &emsp; 1111 &emsp; 10,0000 &emsp; 11,1111 &emsp; 10,1111,1110 &emsp; 
1111,1111,1111,1111 &emsp; 1001,1111,1100,0000,0101,1101 &emsp; 
111,1100,1100,1111,1111,1110,1111,1111  
2. 快速说出以下十进制数所对应的二进制数和十六进制数  
1/1 &emsp; 11/3 &emsp; 101/5 &emsp; 111/7 &emsp; 1001/9 &emsp; 1011/B &emsp; 1101/D &emsp; 1111/F  
0/0 &emsp; 10/2 &emsp; 100/4 &emsp; 110/6 &emsp; 1000/8 &emsp; 1010/A &emsp; 1100/C &emsp; 1110/E
### 检测点1.6
Windows11可以在开始菜单或搜索框中输入“计算器”，然后在左上角菜单中选择“程序员”  
1. FFCH：4092D/1111,1111,1100B
2. FFCH乘以27C0H：27B,6100H/10,0111,1011,0110,0001,0000,0000B
### 第1章习题
1. <table>
   <tr>
      <td align="left"><ins>5</ins>D</td>
      <td align="left"><ins>C</ins>H</td>
      <td align="left"><ins>15</ins>D=<ins>1111</ins>B</td>
   </tr>
   <tr>
      <td align="left"><ins>12</ins>D=<ins>1100</ins>B</td>
      <td align="left"><ins>10</ins>D=<ins>1010</ins>B</td>
      <td align="left"><ins>8</ins>H=<ins>1000</ins>B</td>
   </tr>
   <tr>
      <td align="left"><ins>11</ins>D=<ins>1011</ins>B</td>
      <td align="left"><ins>14</ins>D=<ins>1110</ins>B</td>
      <td align="left"><ins>16</ins>D=<ins>1 0000</ins>B</td>
   </tr>
   </table>

2. <ins>12</ins>H &emsp; <ins>1 0101</ins>B &emsp; <ins>1000 1111</ins>B &emsp; <ins>10 0000 0000</ins>B &emsp; <ins>1FF</ins>H  
# 第2章
### 第2章习题
- 0 &emsp; FFFFF &emsp; $2^{20}$ &emsp; 1024 &emsp; 1
# 第3章
### 检测点3.1
1. 一个字含有（ 2 ）字节和（ 16 ）比特，一个双字含有（ 4 ）字节、（ 2 ）个字和（ 32 ）比特。
2. 二进制数1000 0000中，位（ 7 ）的那个比特是“1”，也就是第（ 8 ）位。<ins>它是最高位。</ins>
3. 一个存储器的容量是16字节，地址范围为（ 0 ）~（ 0FH ）。用该存储器保存字数据时，可存放（ 8 ）个字，这些字的地址分别是（ 0 2 4 6 8 0AH 0CH 0EH ）。<ins>保存双字则为 0 4 8 0CH。</ins>
### 检测点3.2
1. INTEL 8086 有AX、BX、CX、DX、SI、DI、BP、SP八款通用寄存器。长度为16比特，2字节。
2. DX的内容是083CH。
### 检测点3.3
1. （ 8 ） （ AX、BX、CX、DX、SI、DI、BP、SP ） （ AH、AL、BH、BL、CH、CL、DH、DL ）
2. （ A ） （ C ） （ DF ）
3. ABCDF
### 第3章习题
1. 64个。1MB/16KB=64
2. 25BC0H~35BBFH。25BC0H+FFFFH=35BBFH
# 第4章
### 检测点4.1
1. 略
2. （ B ）（ A ）（ C ）
### 第4章习题
（1） 分别为0、35H、40H。  
如图4-8，  
源程序第1行第1个字符m的编码在第一行第一个，为6D，偏移量是0  
源程序第2行第1个字符a的编码在第四行第六个，为61，偏移量是35H  
源程序第3行第1个字符a的编码在第五行第一个，为61，偏移量是40H  
（2） 73字节。  
程序最后一个字符的偏移量是48H，0~48H共49H=73字节
# 第5章
### 检测点5.1
1. （ 0 ）（ 0 ）（ 1 ）（ 0 ）（ 0 ）（ 1 ）
2. ABCD
### 检测点5.2
1. 如果出现了“operation size not specified”的错误提示，可以试试在第3，4，5行的mov后面加上byte  
   即
   ```x86asm
   mov byte [0x00],'a'
   mov byte [0x02],'s'
   mov byte [0x04],'m'
   ```
2. 略
3. 屏幕上显示了`asm`3个字符
# 第6章
### 检测点6.1
1. （ 0xb8000 ）( 0xb800 )（ 0xf9e ）（ 0x48 ）（ 0x27 ）  
   一行160字符，25行一共4000字节，4000=0xfa0，而0xfa0-2=0xf9e就是最后一个字符的偏移量，先写入字符的ASCII码，再写入字符的显示属性  
   'H'的ASCII码为0x48，绿底白字为0010,0111B=27H
2. ABCDIK  
   A：al只有8比特，而0x55aa有16比特，数据宽度不同。如果保持这样写也能编译成功，但效果等同于`mov al,0xaa`  
   B：不能直接把立即数传送给段寄存器，需要先传送给寄存器，寄存器再传送给段寄存器  
   C：ds有16比特，而al只有8比特，数据宽度不同  
   D：没有指定操作大小，0x55aa既可以按word操作，也可以按dword（双字）操作  
   I：ax有16比特，而bl只有8比特，数据宽度不同  
   K：处理器没有在两个内存单元之间直接进行传送的指令  
   注：G会忽略word，效果等同于`mov [0x0a],ax`，但改成`mov byte [0x0a],ax`就会报错
### 检测点6.2
- 0xf000处出现警告，如果不修改，将编译为00  
  实际编译结果为：
  ```x86asm
  1 00000000 55000F                  data1 db 0x55,0xf000,0x0f
  1          ******************       warning: byte data exceeds bounds [-w+number-overflow]
  2 00000003 38002000AA55            data2 dw 0x38,0x20,0x55aa
  ```
### 检测点6.3
1. 执行后AX中的内容是0x210E。
2. 段内偏移地址为0x0030，物理内存地址为0x90230。
3. BFGHIJ  
   B：没有指定操作大小，既可以是byte也可以是word  
   F：没有指定操作大小  
   G：xor的目的操作数不能是通用寄存器或内存单元  
   H：add的目的操作数只能是通用寄存器或内存单元  
   I：div的操作数只能是通用寄存器或内存单元  
   J：add无法将8位寄存器加给16位寄存器  
4. 如果执行div bh，那么AX=0x0001，BX=0x9000，DX=0x0001  
   如果执行div bx，那么AX=0x0001，BX=0x9000，DX=0x7090
### 检测点6.4
- （ E9 02 00 ）  
- （ EA 05 00 00 20 ）
### 检测点6.5
- 略
### 第6章习题
1. 问题在于21015除以10后，商2101大于al的最大上限255即0xff。修正后的代码如下：  
   ```x86asm
   mov ax,21015
   xor dx,dx
   mov bx,10
   div bx
   and cl,0xf0
   ```
2. 将第37行的`mov ax,number`修改为`mov ax,infi`
   显示infi的偏移地址为`299D`即`0x12b`
3. 使用`db 0xcd,0x88`
# 第7章
### 检测点7.1
- （ A ）（ B ）（ D ）（ C ）（ F ）（ E ）（ I ）（ H ）（ G ）
### 检测点7.2
- CE  
  原因：在8086cpu上，只能使用BX、SI、DI、BP来提供偏移地址
### 检测点7.3
- 0xf0=-16 &emsp; 0xff=-1 &emsp; 0x81=-127
- 0xffff=-1 &emsp; 0x8a08=-30200
### 检测点7.4
1. （ 1 ）（ 1 ）（ 0 ）（ 1 ）（ 0 ）（ 0 ）（ 0 ）（ 0 ）（ 0 ）  
   当ZF=1时，表明计算结果为零；  
   而jz完全等价于je，它们对应同一个操作码，jnz和jne同理  
   jz或je指令的意思是当ZF=1，即计算结果为0时转移；  
   jnz或jne指令的意思是当ZF=0，即计算结果非0时转移；  
2. ```x86asm
   cmp ax,bx
   ja  lbb
   je  lbz
   jb  lbl
   ```
### 检测点7.5
- 略
### 第7章习题
1. 正数7个，负数6个  
   - 正数：  
     - 0x05 0x30
     - 0x90 0xa0 0x1235 0x2f 0xc0
   - 负数：
     - 0xff 0x80 0xf0 0x97
     - 0xfff0 0xc5bc
2. 见github源文件[xt7-2.asm](https://github.com/sishuikaki/assembly_study/blob/main/xt7-2.asm)
3. 65536次，即0x10000次  
   cx=0，减去1次1后变成`...1111 1111 1111`，此时loop判断cx非0，跳转到delay，再减去1111,1111b次1后变成`...1111 0000 0000`，此时cx再一次等于0，loop跳出循环  
   1111 1111b=65535，65535+1=65536
# 第8章
### 检测点8.1
1. ax=0xfff0  
   `and [data],ax`后data的内容为0xaa50  
   `or ax,[data]`后ax不变
2. AC  
   B错误，是先访问栈段，读取栈顶数据，再将SP的内容减2。出栈是入栈的反向操作
3. ```x86asm
   push ds
   push bx
   push ax
   mov bx,ss
   mov ds,bx   ;将ss赋值给ds
   mov bx,sp
   mov dx,[bx] ;此时ds:bx等同于ss:sp
   pop ax
   pop bx
   pop ds
   ```
### 第8章习题
1. 修改后
   ```x86asm
   ;以下计算1到100的和 
   xor ax,ax
   mov cx,100
   @f:
   add ax,cx
   loop @f
   ```
2. 见github源文件[xt8-2.asm](https://github.com/sishuikaki/assembly_study/blob/main/xt8-2.asm)  
   不足：1+2+...+1000=500500，除以10后小于65535，ax能够保存商，此时无需考虑除法溢出；  
   但如果累加和的数值除以10后大于65535，ax不够保存商，此时会发生除法溢出；  
   *如果感兴趣可以参考王爽的《汇编语言》一书中实验10的2. 解决除法溢出的问题。（注意：MASM和NASM语法有些许差异）*
# 第9章
### 检测点9.1
1. 0x70
2. 0x80
3. 0
> data1的vstart=0，lba相对于data1起始处的距离为0  
> 注意`mov ax,lba`和`mov ax,[lba]`的区别  
> 如果是`mov ax,lba`，那么ax将等于ds:[0]的内容
4. 2
> data2的vstart=0，lbc相对于data2起始处的距离为2
5. 0x80
> data3没有说明vstart=0，lbd相对于整个程序开头的距离为0x80
### 检测点9.2
1. `call label_proc`
2. `call bx`
3. `call [bx]`
4. `call 0xf000:0x0002`
5. `call far [0x80]`
6. `call far [bx+di+0x08]`
### 检测点9.3
1. ax=0x2a95
2. &nbsp;  
   - a. `jmp label_proc`  
   - b. `jmp bx`  
   - c. `jmp [es:bx]`  
      > 注意是附加段

   - d. `jmp 0xf000:0x0002`  
   - e. `jmp far [0x80]`  
   - f. `jmp far [es:bx+di+0x08]`
### 第9章习题
1. 可以将第150到第154行代码改为
   ```x86asm
   mov ax,[es:code_2_segment]
   mov [gotocode_2+2],ax
   jmp far [gotocode_2]
   gotocode_2 dw begin,0
   ```
2. 如果用户程序的实际长度小于等于512个字节，那么加载程序无法正常运行  
   cx初始为0，执行一次`loop @2`后，cx变为0xffff，继续循环  
   在`loop @2`这条命令设置断点后，按c即可进入下一次循环，观察每次运行到`loop @2`时ds或ax的值  
   在循环到ds=0xb800时，屏幕文字将开始依次消失（ASCII码全为0）  
   在循环到ds=0xfffe时，下一次循环时ds将会变成0  
   在循环到ds=0x07a0时，下一次循环时0x7c00的指令被替换，加载程序无法正常运行
# 第10章
### 检测点10.1
- 略
### 检测点10.2
- 使用`help xp`查看xp命令的使用方法
- 使用`xp /512bx 0`查看内存中0:0-0:200的数据
  > 512：512个，b：字节，x：16进制。512bx就是以16进制显示512个字节，0：从地址0x0开始

- 使用`xp /4bx 0x1c0`查看0x70号中断处理过程的段地址和偏移地址
  > 0x70*4=0x1c0

### 