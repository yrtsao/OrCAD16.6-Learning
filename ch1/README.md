Crate a file  

File > New > Project  
在New Project 窗口（见图1. 1） 中， 输入项目名称， 并且从四种项目类型  
中选择一种作为本项目的类型：  
· Analog or Mixed A / D 用于PSpice 仿真。  
	么选择Analog or Mixed A / D 作为项目类型，   
这样就会激活Capture 顶部工具栏的PSpice 菜单。  
	
· PC Board Wizard 用于PCB 项目中的原理图绘制。  
· Programmable Logic Wizard 用于CPLD 和FPGA 设计。  
· Schematic 用于原理图绘制。  





符号  
符号不是通过Place Part 菜单在原理图中进行放置。他们通过Place 菜单（见图1. 8） 选择符号直接放置。  
放置电源符号的快捷键为F， 当按下F 键时， Place Power 放置电源菜单将会弹出  



PSpice 仿真软件中包括source 和capsym 两个符号库。  
Capsym 库包含所有模拟地和电源符号  
source 库也包含模拟0V 符号  
	D_HI 数字高符号和D_LO 数字低符号， 它们分别用来设置导线或数字器件的高低电平值。  
	
	
元器件  

通过选择Place > Part 菜单命令进行元器件放置。  
各种网络连接符号通过Place 菜单进行放置， 而实际元件通过Place > Part 菜单进行放置。 元件库Part 和符号库Symbol 的扩展名均为. olb， 为其图形显示， 用于软件绘图。  







放置PSpice 元器件  
该功能可以快速放置通用的PSpice 元器件， 而不用再查找半导体供应商的元器件号码。  
通过顶层工具栏的Place 菜单放置元器件  
	无源元件来自analog 库  
	电位器却保存在breakout 库  





通用的半导体器件具有默认的名称和参数， 可以通过PSpice Model Editor 对其进行个性化设置， 但是演示版只能对二极管模型进行编辑。  


通过PSpice Model Editor 对其进行个性化设置， 但是演示版只能对二极管模型进行编辑。  
对Breakout 器件库中的半导体器件进行个性化设置主要用于高级电路， 此时需要对半导体的特性参数进行配置。  


创建项目时另一个常见的错误就是项目类型选择错误  
如下操作修改项目类型： 选定项目管理器中的Design Resources， 然后通过单击右键rmb > Change Project Type 进行项目类型修改  

作業1 截圖  
![image](https://github.com/yrtsao/OrCAD16.6-Learning/assets/82528634/bd89fceb-fc42-49f6-a1e5-1bc71c573d7f)
