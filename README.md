# gcc
Explore, study, theory; Gimple, three-address, SSA, Register-Transfer Level, RTL, .md files (machine description), code generation, lowering ...

* gccjit
 
https://gcc.gnu.org/onlinedocs/jit/



https://github.com/gcc-mirror/gcc/blob/master/gcc/config/i386/i386.opt

https://github.com/gcc-mirror/gcc/blob/master/gcc/config/i386/i386.md

https://github.com/gcc-mirror/gcc/blob/master/gcc/config/i386/athlon.md


https://gcc.gnu.org/onlinedocs/jit/internals/index.html#environment-variables

```

 /* Indentation indicates inheritance: */
  class context;
  class memento;
    class string;
    class location;
    class type;
      class function_type;
      class compound_type;
        class struct_;
	class union_;
      class vector_type;
      class array_type;
    class field;
      class bitfield;
    class fields;
    class function;
    class block;
    class rvalue;
      class lvalue;
        class local;
	class global;
        class param;
      class base_call;
      class function_pointer;
    class statement;
      class extended_asm;
    class case_;
    class memento_of_get_aligned;
  class top_level_asm;

```

* **libgccjit.so**

When the context is compiled, the gcc::jit::playback classes (within jit-playback.cc and jit-playback.h) replay the API calls within langhook:parse_file:
```
  /* Indentation indicates inheritance: */
  class context;
  class wrapper;
    class type;
      class compound_type;
    class field;
    class function;
    class block;
    class rvalue;
      class lvalue;
        class param;
    class source_file;
    class source_line;
    class location;
    class case_;
```
```
gcc::jit::recording::context

...

@P1
... /c/gccjit/

gccjit gcc-13 \
    jit1.cc \
    -o 1.exe \
    -lgccjit \
     -L/usr/lib/gcc/x86_64-linux-gnu/ \
    -I/usr/lib/gcc/x86_64-linux-gnu/13/include/ \
   -lstdc++ -Wall

./1.exe
```


## gccjit

https://gcc.gnu.org/onlinedocs/jit/cp/topics/objects.html
https://gcc.gnu.org/onlinedocs/jit/topics/functions.html
https://gcc.gnu.org/onlinedocs/jit/cp/intro/tutorial04.html
https://gcc.gnu.org/onlinedocs/jit/cp/topics/functions.html#_CPPv4N6gccjit8function11dump_to_dotEPKc
https://gcc.gnu.org/onlinedocs/jit/cp/topics/functions.html#_CPPv4N6gccjit5case_E
https://gcc.gnu.org/onlinedocs/jit/cp/intro/tutorial03.html
https://gcc.gnu.org/onlinedocs/jit/cp/topics/expressions.html#_CPPv4N6gccjit6rvalueE



