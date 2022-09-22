# Continuous Learning :: leveldb #

## 一、构建和编译

1. 代码分支：[google/leveldb - tag:1.23](https://github.com/google/leveldb/tree/1.23)
2. `leveldb` 采用 `cmake` 工具进行构建，可以直接构建和编译
    ```shell
    $ mkdir -p ./build/
    $ cmake -DCMAKE_BUILD_TYPE=Debug -DCMAKE_C_COMPILER=$(which clang) -DCMAKE_CXX_COMPILER=$(which clang++) -S . -B ./build/ -G Ninja
    $ cmake --build ./build/ --parallel 16
    ```