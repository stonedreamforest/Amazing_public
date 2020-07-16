# Amazing_public
自动监控目标程序执行任意指令,指令级辅助分析反调试(如int2e)、反虚拟机（如cpuid）、加密算法、程序破解... 


#### 使用

1. 下载pin、下载Amazing 解压到任意目录
2. 将目录下的`pinhlper.dll`移动至pin文件夹的`IA32\BIN\`目录下
3. 在`bin\msvc32`目录打开`haloamazing.exe`
![image](https://user-images.githubusercontent.com/16742566/87127052-d7020f80-c2bf-11ea-87c5-78da90862201.png)
    - 模式
      - once:只监控第一次执行的指令
      - full：监控所有执行指令
   
4. 点击`HALOAMAZING`启动 


#### 效果


![qqtROglKNq](https://user-images.githubusercontent.com/16742566/87137741-fc971500-c2cf-11ea-8bd7-36c3000a39bf.gif)


#### 数据缓存（sqlite）
> 可通过python与ida、ghidra、binary ninja交互
- 部分视图
    - 反汇编
    ![image](https://user-images.githubusercontent.com/16742566/87556522-555c1880-c6e9-11ea-8cce-621393ad07f5.png)

    - 寄存器
    ![image](https://user-images.githubusercontent.com/16742566/87556773-9f44fe80-c6e9-11ea-89e2-e8af26c0de11.png)

- 使用
    - 查看执行过的rdtsc指令
    ![image](https://user-images.githubusercontent.com/16742566/87668927-a3cbee80-c79f-11ea-8ee7-18f3bbcc9d31.png)


#### 依赖
- 主要依赖于`pin` + `WPF(.net framework 4.8)`
