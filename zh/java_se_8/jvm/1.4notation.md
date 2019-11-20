#### 1.4 Notation

Throughout this specification we refer to classes and interfaces drawn from the Java SE platform API. Whenever we refer 
to a class or interface (other than those declared in an example) using a single identifier N, the intended reference is 
to the class or interface named N in the package java.lang. We use the fully qualified name for classes or interfaces 
from packages other than java.lang.

Whenever we refer to a class or interface that is declared in the package java or any of its subpackages, the intended 
reference is to that class or interface as loaded by the bootstrap class loader (§5.3.1).

Whenever we refer to a subpackage of a package named java, the intended reference is to that subpackage as determined by 
the bootstrap class loader.

The use of fonts in this specification is as follows:

- A fixed width font is used for Java Virtual Machine data types, exceptions,errors, class file structures, Prolog code, and Java code fragments.
- Italic is used for Java Virtual Machine "assembly language", its opcodes and operands, as well as items in the Java Virtual Machine's run-time data areas. It is also used to introduce new terms and simply for emphasis.

Non-normative information, designed to clarify the specification, is given in smaller, indented text.
    
    This is non-normative information. It provides intuition, rationale, advice, examples, etc.
