public class Hellow {
	
}# 访问控制	
				private	私有的
				protected	受保护的
				public	公共的
				default	默认
# 类、方法和变量修饰符	
				abstract	声明抽象
				class	类
				extends	扩充,继承
				final	最终值,不可改变的
				implements	实现（接口）
				interface	接口
				native	本地，原生方法（非 Java 实现）
				new	新,创建
				static	静态
				strictfp	严格,精准
				synchronized	线程,同步
				transient	短暂
				volatile	易失
# 程序控制语句	
				break	跳出循环
				case	定义一个值以供 switch 选择
				continue	继续
				default	默认
				do	运行
				else	否则
				for	循环
				if	如果
				instanceof	实例
				return	返回
				switch	根据值选择执行
				while	循环
# 错误处理	
				assert	断言表达式是否为真
				catch	捕捉异常
				finally	有没有异常都执行
				throw	抛出一个异常对象
				throws	声明一个异常可能被抛出
				try	捕获异常
				包相关	import	引入
				package	包 
# 基本类型	
				boolean	布尔型
				byte	字节型
				char	字符型
				double	双精度浮点
				float	单精度浮点
				int	整型
				long	长整型
				short	短整型
# 变量引用	
				super	父类,超类
				this	本类
				void	无返回值
# 保留关键字	
				goto	是关键字，但不能使用
				const	是关键字，但不能使用
				null	空


> 所有java程序都是从void开始

> 	对象：对象是类的一个实例，有状态和行为。例如，一条狗是个对象，它的状态 有：颜色、名字、品种；行为有：摇尾巴、叫、吃等。

> 类：类是一个模板，它描述一类对象的行为和状态。

> 方法：方法就是行为，一个类可以有很多方法。逻辑运算、数据修改以及所有动作都是在方法中完成的。

> 实例变量：每个对象都有独特的实例变量，对象的状态由这些实例变量的值决定。

>  public static void main (String [] arige){

> 局部变量：在方法、构造方法或者语句块中定义的变量被称为局部变量。变量声明和初始化都是在方法中，方法结束后，变量就会自动销毁。--dog.java

# 构造方法

每个类都有构造方法。如果没有显式地为类定义构造方法，Java编译器将会为该类提供一个默认构造方法。

在创建一个对象的时候，至少要调用一个构造方法。构造方法的名称必须与类同名，一个类可以有多个构造方法。

>实例化：使用关键字new来创建一个对象。

>初始化：使用new创建对象时，会调用构造方法初始化对象。

> 构造方法是一种特殊的方法，它是一个与类同名的方法。对象的创建就是通过构造方法来完成，其功能主要是完成对象的初始化。当类实例化一个对象时会自动调用构造方法。构造方法和其他方法一样也可以重载。

1.构造方法作用：（1）.构造出来一个类的实例 （2）.对构造出来个一个类的实例（对象）初始化。

2.构造方法的名字必须与定义他的类名完全相同，没有返回类型，甚至连void也没有。

3.主要完成对象的初始化工作，构造方法的调用是在创建一个对象时使用new操作进行的。

4.类中必定有构造方法，若不写，系统自动添加无参构造方法。接口不允许被实例化，所以接口中没有构
造方法。

5.不能被static、final、synchronized、abstract和native修饰。

6.构造方法在初始化对象时自动执行,一般不能显式地直接调用.当同一个类存在多个构造方法时，java编译系统会自动按照初始化时最后面括号的参数个数以及参数类型来自动一一对应。完成构造函数的调用。

7.构造方法分为两种：无参构造方法 有参构造方法


# 访问实例变量和方法 --pippy1
通过已创建的对象来访问成员变量和成员方法，如下所示：

> /* 实例化对象 */
Object referenceVariable = new Constructor();

>/* 访问类中的变量 */
referenceVariable.variableName;

>/* 访问类中的方法 */
referenceVariable.methodName();


> 类变量：独立于方法之外的变量，用 static 修饰。

> 实例变量：独立于方法之外的变量，不过没有 static 修饰。

> 局部变量：类的方法中的变量。

# main 函数是静态，无法直接访问变量，通过new来实例访问

# static 为静态 ，表示他没有对象  静态变量会储存 ， 每次使用会继承上一次的值 。

# 非静态的变量每次使用都会重置