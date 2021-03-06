## 第8章 函数探幽
- 内联函数
	- 内联函数的编译代码与其他程序代码“内联”起来了。也就是说编译器将使用相应的函数代码替换函数调用。
	- 对于内联代码，程序无需跳到另外一个位置执行代码，再跳回来。
	- 因此，内联函数的运行速度比常规函数稍快，但代价需要占用更多内存。
	- 使用内联函数
		- 在函数声明前加上关键字inline
		- 在函数定义前加上关键字inline
- 默认参数
	- 设置参数默认值，必须通过函数原型。
	- 由于编译器通过查看原型来了解函数所是用的参数数目，因此函数原型也必须将可能的默认参数告知程序。
- 函数重载
	- 函数重载的关键是函数的参数列表-也称为函数特征标（function signature）。
	- 如果两个函数的参数数目和类型相同，同时参数的排列顺序也相同，则他们的特征标相同，而变量名是无关紧要的。
	- C++允许定义名称相同的函数，条件是他们的特征标不同。
	- 编译器在检查函数特征标时，将把类型引用和类型本身视为同一个特征标。
- 函数模板
	- 函数模板是通用的函数描述，也就是说，他们使用泛型来定义函数。

			template <typename AnyType> //C++98新增typename关键字
            template <class AnyType>
	- 编写模板函数很可能无法处理某些类型。
	- 显式具体化
		- 对于给定的函数名，可以有非模板函数、模板函数和现实具体化模板函数以及他们的重载版本。
		- 显式具体化的原型和定义以`template <>`打头，并通过名称来指出类型。
		- 具体化优先于常规模板，而非模板函数优先于具体化和常规模板。
	- 函数模板自动完成重载函数的过程。只需要使用泛型和具体的算法来定义函数，编译器将为程序中使用的特定参数类型生成正确的函数定义。