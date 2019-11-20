#### Preface to the Java SE 8 Edition

THE Java SE 8 Edition of The Java® Virtual Machine Specification incorporates all the changes that have been made to the
Java Virtual Machine since the Java SE 7 Edition in 2011. In addition, numerous corrections and clarifications have been 
made to align with popular implementations of the Java Virtual Machine.

This Edition continues the tradition of specifying the abstract Java Virtual Machine, serving as documentation for a 
concrete implementation only as a blueprint documents a house. An implementation of the Java Virtual Machine must embody
this specification, but is constrained by it only where absolutely necessary.

Notable changes to the Java programming language in Java SE 8 have brought corresponding changes to the Java Virtual 
Machine. To maximize binary compatibility, it has been desirable to specify default methods directly in the Java Virtual 
Machine, rather than relying on compiler magic that might not be portable across vendors or product releases, and is 
certainly not applicable to pre-existing class files. In the context of JSR 335, Lambda Expressions for the Java 
Programming Language, Dan Smith at Oracle consulted with implementers to determine how best to integrate default methods 
into the constant pool and method structures, the method and interface method resolution algorithms, and the bytecode 
instruction set. JSR 335 also introduced private and static methods in interfaces at the class file level; they too have 
been carefully integrated with interface method resolution.

A theme of Java SE 8 is co-evolution of the Java SE platform libraries with the Java Virtual Machine. A small but useful 
example is support for method parameter names at run time: storing such names in the class file structure goes hand in 
hand with offering a standard API to retrieve them (java.lang.reflect.Parameter). This illustrates an interesting 
development in the class file structure over the years: the First Edition of this specification defined six attributes, 
of which three were deemed critical to the Java Virtual Machine, while this Java SE 8 Edition defines 23 attributes, 
of which five are deemed critical to the Java Virtual Machine; that is to say, attributes now exist primarily to support 
libraries and tools rather than the Java Virtual Machine itself. To help readers understand the class file structure, 
this specification more clearly documents the role of each attribute and the constraints placed upon it.

Many colleagues in the Java Platform Group at Oracle have provided valuable support to this specification: Mandy Chung, 
Joe Darcy, Joel Borggrén-Franck, Staffan Friberg, Yuri Gaevsky, Jon Gibbons, Jeannette Hung, Eric McCorkle, Matherey 
Nunez, Mark Reinhold, John Rose, Georges Saab, Steve Sides, Bernard Traversat, Michel Trudeau, and Mikael Vidstedt. 
Particular thanks to Dan Heidinga (IBM), Karen Kinnear, Keith McGuigan, and Harold Seigel for their ironclad commitment 
to compatibility and security in popular Java Virtual Machine implementations.

Alex Buckley
Santa Clara, California 
March, 2014