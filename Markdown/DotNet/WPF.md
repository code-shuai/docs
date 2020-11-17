# WPF 
**（Windows Presentation Foundation）**
WPF 界面 底层使用DirectX ，特定服务 依赖于User32

### 1.5 WPF 4.5

WPF 是一种成熟的技术。它是几个已经发布的DotNet 平台的一部分  
WPF 3.0  
.Net Framework 3.0 三大新技术
WPF(Windows Presentation Foundation)
WCF(Windows Communication Foundation)
WF(Workflow Foundation)
WPF 3.5
一年后，一个新的版本作为 .Net Framework 3.5 的一部分发布。
新版本WPF 的新特性主要是一些小的改进，包括错误修复和性能改进
WPF 3.5 SP1
WPF 4
WPF 4.5   


------

**14 **

#### 1.5.1 WPF 工具包

#### 1.5.2 Visual Studio 2012

1. 多目标

------

**15 （第1章 WPF概述 ）**

2. Visual Studio 设计器

------

**16 （第1部分 基础知识）**

### 1.6 小结

**17**

## 第 2 章  XAML

  ML（Extensible Application Markup Language）（读音“zammel”）用于实例化.Net对象的标记语言。尽管XAML 是一种可应用于诸多不同问题领域的技术，但其主要作用是构造WPF用户界面。换言之，XAML文档定义了在WPF应用程序中组成窗口的面板、按钮及各种控件的布局。
  再手动编写XAML，可使用工具生成所需的XAML。如果您是一位图形设计人员，该工具可能是图形设计程序，如Expression Blend。如是一名卡法人员，Microsoft Visual Studio。。。。。。
  将详细介绍XAML，分析XAML的作用、宏观体系结构及语法。

### 2.1 理解 XAML

开发人员很久前就已经意识到,要处理图形丰富的复杂应用程序,最有效的方式是将图形部分从底层的代码中分离出来。这样一来,美工人员可独立地设计图形,而开发人员可独立地编写代码。这两部分工作可单独地进行设计和修改,而不会有任何版本问题。

#### 2.1.1 WPF 之前的图形用户界面

#### 2.1.2 XAML 变体

	WPF XAML
	XPS XAML 
	Silverlight XAML
	WF XAML

#### 2.1.3 XAML 编译

### 2.2 XAML 基础

- XAML 文档中的每个元素都映射为 .NET 类的一个实例。元素名称也完全对应类名。
- 与所有XML 文档一样，可在一个元素中嵌套另一个元素。（嵌套表示“包含” ）
- 可通过特性（attribute）设置每个类的属性（property）。特殊情况特殊语法使用嵌套的标签（tag）

**XAML 文档基本框架，该文档表示一个新的空白窗口**

```xaml
<Window x:Class="StudyWPF.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:StudyWPF"
        mc:Ignorable="d"
        Title="MainWindow" Height="450" Width="800">
    <Grid>

    </Grid>
</Window>
```

#### 2.2.1 XAML 名称空间





