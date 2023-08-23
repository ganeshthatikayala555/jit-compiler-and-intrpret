# jit-compiler-and-intrpret

Here we provide a java code to tell how jit compiler works and interpretation is done 
when java code conveted to bytecode by javac and is taken to another machine for execution,the byte code is interpreted first  
At the beginning, when the program starts running, the JVM interprets the bytecode of the entire program. 
the loop and its calculation are interpreted, which might be slower compared to native machine code execution.
 As the program continues to execute, the JIT compiler recognizes that the loop is a hotspot since it's executed repeatedly. 
 The JIT compiler optimizes the loop by compiling it into native machine code. The calculation of the sum is more efficiently performed in native code.

Mix of Execution: While the loop is compiled into native machine code and executed efficiently, other parts of the program,
such as variable declarations and the print statement, might still be interpreted.
n this example, the loop that calculates the sum is a hotspot that gets compiled into native machine code by the JIT compiler,
while other parts of the program might continue to be interpreted by the JVM. 
l
