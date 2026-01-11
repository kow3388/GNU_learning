# GNU
GNU是一個軟體專案提供一整套C/C++開發工具鏈  

C/C++ 執行 & 開發流程
```
編譯 -> 組譯 -> 連結 -> 執行/除錯/建置
```
對應到GNU的工具:  
1. 編譯 (compile) -> gcc/g++ (GNU compiler)  
   把high level language (e.g. C/C++) 翻成 assembly (組合語言)  

2. 組譯 (assemble) -> as (GNU assembler)  
   把assembly翻成machine language  

3. 連結 (link) -> ld (GNU link loader)  
   把多個翻譯成machine language的檔案 + library變成一個可執行檔  

4. C library -> glibc (GNU C library)  
   C的標轉函式庫  

5. 除錯 (debug) -> gdb (GNU debuger)  
   提供開發者debug工具  

6. 建置 (make) -> make (GNU makefile)  
   自動化的編譯工具，即可不用每次都打一大堆指令  

因為GNU的gcc/g++把compile, assemble和link整合在一起，因此實際上開發者實際會需要學習使用的部份是gcc/g++, gdb和make