# assembly_study
学习 王爽《汇编语言（第3版）》 时编写的复杂程序
## exp7.asm
实验7 P172
## exp9.asm
实验9 P187
## exp10_1.asm exp10_2.asm exp10_3.asm
实验10 P206
## des1.asm
课程设计1 P211
## exp11.asm
实验11 P234
## exp12.asm
实验12 P251
## exp13_1.asm exp13_2.asm exp13_3.asm
实验13 P262
## exp14.asm
实验14 P271
## exp15.asm
实验15 P285
## exp16.asm
实验16 P299  
此实验有个重要的地方  
地址标号和数据标号记录的都是程序运行时，标号位置的绝对偏移地址  
但是安装到0:200h后，转移指令的那些标号的地址并没有改变  
所以需要使用`相对位移 + 绝对地址200h`的形式  
