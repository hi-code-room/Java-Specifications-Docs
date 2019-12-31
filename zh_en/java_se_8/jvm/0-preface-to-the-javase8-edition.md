#### Preface to the Java SE 8 Edition

#### Java SE 8 版前言

​		THE Java SE 8 Edition of The Java® Virtual Machine Specification incorporates all the changes that have been made to the Java Virtual Machine since the Java SE 7 Edition in 2011. In addition, numerous corrections and clarifications have been made to align with popular implementations of the Java Virtual Machine.

​         Java® 虚拟机规范的 Java SE 8 版包含自 2011年 Java SE 7 版以来对 Java 虚拟机所做的所有更改。此外，为了与 Java 虚拟机的流行实现保持一致进行了大量的更正和澄清。

​		This Edition continues the tradition of specifying the abstract Java Virtual Machine, serving as documentation for a concrete implementation only as a blueprint documents a house. An implementation of the Java Virtual Machine must embody this specification, but is constrained by it only where absolutely necessary.

​		此版本延续了特定抽象 Java 虚拟机的传统，如同房屋的蓝本一样作为具体实现的文档。Java 虚拟机的实现必须体现此规范，但仅在绝对必要时受其约束。

​		Notable changes to the Java programming language in Java SE 8 have brought corresponding changes to the Java Virtual Machine. To maximize binary compatibility, it has been desirable to specify default methods directly in the Java Virtual Machine, rather than relying on compiler magic that might not be portable across vendors or product releases, and is certainly not applicable to pre-existing class files. In the context of JSR 335, Lambda Expressions for the Java Programming Language, Dan Smith at Oracle consulted with implementers to determine how best to integrate default methods into the constant pool and method structures, the method and interface method resolution algorithms, and the bytecode instruction set. JSR 335 also introduced private and static methods in interfaces at the class file level; they too have been carefully integrated with interface method resolution.

​		Java SE 8 中 Java 编程语言的显著变化给 Java 虚拟机带来了相应的更改。为了最大化二进制兼容性，最好直接在 Java 虚拟机中指定默认方法，而不是依赖可能无法跨供应商或产品版本可移植的编译器魔力，并且肯定不适用于预先存在的类文件。在 JSR 335 上下文中，Java 编程语言中的 Lambda 表达式，Oracle 的 Dan Smith 咨询了实现者，以确定如何最好地将默认方法集成到常量池和方法结构、方法和接口方法中解析算法和字节指令集。JSR 335还在类文件级别的接口中引入了私有和静态方法，他们也经过精心集成与接口方法解析。

​		A theme of Java SE 8 is co-evolution of the Java SE platform libraries with the Java Virtual Machine. A small but useful example is support for method parameter names at run time: storing such names in the class file structure goes hand in hand with offering a standard API to retrieve them (java.lang.reflect.Parameter). This illustrates an interesting development in the class file structure over the years: the First Edition of this specification defined six attributes, of which three were deemed critical to the Java Virtual Machine, while this Java SE 8 Edition defines 23 attributes, of which five are deemed critical to the Java Virtual Machine; that is to say, attributes now exist primarily to support libraries and tools rather than the Java Virtual Machine itself. To help readers understand the class file structure, this specification more clearly documents the role of each attribute and the constraints placed upon it.

​		Java SE 8 的一个主题是与 Java 虚拟机共同演进 Java 平台库。一个小但是有用的示例是在运行时支持方法参数名：在类文件结构存储此类名称与提供标准 API 以检索它们（Java.lang.relfect.Parameter）是齐头并进的。这说明多年来类文件结构的一个有趣的发展过程：此规范的第一版定义了6个属性，其中三个被认为对 Java 虚拟机至关重要，而此 Java SE 8 版本定义了23 个属性，其中5个属性被认为对 Java 虚拟机至关重要；也就是说，属性现在主要用于支持库和工具，而不是 Java 虚拟机本身。为了帮助读者了解类文件结构，此规范更清楚地记录了每个属性的作用以及施加的约束。

​		Many colleagues in the Java Platform Group at Oracle have provided valuable support to this specification: Mandy Chung, Joe Darcy, Joel Borggrén-Franck, Staffan Friberg, Yuri Gaevsky, Jon Gibbons, Jeannette Hung, Eric McCorkle, Matherey Nunez, Mark Reinhold, John Rose, Georges Saab, Steve Sides, Bernard Traversat, Michel Trudeau, and Mikael Vidstedt. Particular thanks to Dan Heidinga (IBM), Karen Kinnear, Keith McGuigan, and Harold Seigel for their ironclad commitment to compatibility and security in popular Java Virtual Machine implementations.

​		Oracle Java 平台小组的许多同事为了这一规范提供了宝贵的支持：Mandy Chung, Joe Darcy、Joel Borggrén-Franck、Staffan Friberg、Yuri Gaevsky、Jon Gibbons, Jeannette Hung、Eric McCorkle、Matherey Nunez、Mark Reinhold, John Rose、Georges Saab、Steve Sides, Bernard Traversat、Michel Trudeau、and Mikael Vidstedt。特别感谢 Dan Heidinga (IBM)、 Karen Kinnear、Keith McGuigan 和 Harold Seigel 在流行 Java 虚拟机的实现中对兼容性和安全性的坚定承诺。		

Alex Buckley

Santa Clara, California 
圣克拉拉 （加利福尼亚州）

March, 2014
2014 年 3 月