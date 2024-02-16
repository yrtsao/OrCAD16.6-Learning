直流工作点分析  

当电路启用工作点计算时， 仿真输出文件中将包含以下数据：   
模拟和数字节点电压值、电压源电流和功率值、所有元件的小信号参数。  
在PSpice 仿真设置中可以对工作点的输出信息进行取舍。  

对电路进行工作点仿真计算时， 所有电容默认为开路， 所有电感默认为短路。  

首先绘制仿真电路图， 然后通过顶部工具栏  
PSpice > New Simulation Profile 对电路进行仿真设置。  
通过该工具栏可以对电路  
进行直流分析、交流分析、瞬态分析和工作点分析设置，   
通常情况下默认仿真类型为工作点分析。  
本例采用默认仿真设置， 通过菜单PSpice > Run 或选择图标运行电路仿真。  

![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/0a8ffe17-99b5-4193-b867-577c2abc16a1)





生成网络表  

Capture 中的电路图以网络表的形式体现， 该网络表中包含所有元件信息及  
元件与元件之间的连接关系。当对电路进行仿真分析时， 程序会自动生成网络  
表， 并把该网络表保存在项目管理器的Outputs folder 输出文件中  
![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/a9d14ba0-285e-48d3-8be4-8065d8164274)

需要注意的是Cap⁃ture 不区分大小写， 任何以大写字母命名的原理图， 其网络表都将以小写字母命  

![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/3304ae5a-e105-4856-b087-8daf7cb3aacf)

双击网络表名称， 网络表的内容就会呈现出来， 如图2. 8 所示。  
图2. 8 所示为原理图的网络表， 电阻R1 连接于节点in 和节点out 之间， 阻值为10Ω， 温度系数为零（TC = 0）。V1 为电压源， 连接于节点in 和0V 之间，  
幅值为10V。  
![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/d3dd2ad4-3692-46f4-94ce-39e14d336329)


当对电路进行直流工作点分析时， 因为没有波形数据， 所以不能进行图形绘制。  
可以通过Output File 输出文件或者原理图查看计算结果，   
包括各元件的偏置电压、电流和瞬时功率。  
通过Capture 或PSpice 顶部工具栏中的View >Output File 菜单可以查看全部输出文件（见图2. 9）。  

![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/83d71f8c-fd74-4f40-9563-e5911bec138d)

菜单选项Options > Preferences > Text Editor 可以对默认颜色进行更改。  

![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/e0904336-2a0b-44ad-ace9-8d913dd25f99)

仿真输出文件提供了一个非常详细的电路分析报告， 包括模拟和数字节点电压、流过元件的电流及小信号参数列表。  

可以通过选项对工作点信息报告进行输出设置。在仿真设置窗口的Category 中选择Output file， 如图2. 11 所示， 并且取消NOBIAS 选项。选定LIST 选项， 输出文件将会列出电路中的所有元件、各连接节点值、参数值、模型型号等参数。  
![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/9692c148-35b4-4afb-9373-b10a19b5d3a3)


　显示工作点数据  

当电路运行仿真之后，   
各节点的偏置电压、电流和功率值都可以在原理图中进行显示。  
在Capture 中， 选择菜单PSpice > Bias Points > Enable 或者通过工作点显示图标对以上信息进行显示。  
图2. 13 显示出RC 电阻电路的偏置电压、电流和瞬时功率。  
如图2. 14 所示， 工作点数值的显示位数可以通过菜单PSpice > Bias Points  
> Preferences 进行修改。到目前为止， 数值的最高准确度为10 位。  

![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/8bc00f49-5dec-46e2-b5bd-3af2ffd40481)


![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/4760b957-219b-471e-a783-5b8d0be40519)

当打开或者关闭工作点显示功能时， 需要通过F5 键对显示信息进行刷新。  




保存工作点数据  
如果使用保存的工作点数值， 必须保证电路的网络表中的信息，  
例如各元件的连接等均没有改变。同样， 其他类型的仿真分析也可以利用工作点数值，  
前提是电路进行再仿真时其网络表没有发生任何改变。  
在Simulation Profile Settings 仿真设置窗口选择Bias Point 工作点分析，  
然后选择Save Bias Point 保存工作点数值。如图2. 15 所示，  
工作点分析的详细数据保存在saved bias point. txt 文本文件中。可以通过Browse. . . 浏览按钮选择或者创建保存该文件的文件夹。  
文本文件中保存的工作点数据主要包括：  
 各节点电压值和电路中所有元件的数字状态、总功率和电压源的电流、电路中所有元件的模型参数。  

![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/dc125818-cc89-49b0-9337-4dbcc7dcb76c)


加载工作点数据  
![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/28521b54-9a8e-4b24-b235-b3de3594eaff)
