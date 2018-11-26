# z3工程在XCode下生成可调试执行文件：
  在工程根目录下：
    1. mkdir build 
    2. 在工程根目录下执行：
        CXX=clang++ CC=clang python scripts/mk_make.py -d
        通过-d指明生成可调试的可执行文件。会在build目录下生成Makefile。
    3. 新建XCode工程，由于使用外部的make构建的，选择External Building System，指明Makefile所在的文件夹即可。

# 其余的编译可用cmake + make 的方式来编译。

# 在VS中的编译调试尚未实验，可以参照README-CMake.md来尝试。
