# インストール方法
```bash
git clone https://github.com/Potewo/PrepareCppProject.github
```
好みに応じてパスの通った場所においたりシンボリックリンクを作ったりしてください。

# 使い方
```bash
mkcpp フォルダ名
```
とすることで今いるディレクトリにそのフォルダ名のフォルダを作り、その中にmain.cppとmakefileを作ります。  
作られたディレクトリ で`make`を実行するとコンパイル 、実行します。
# 作られるファイル
**main.cpp**
```c++
#include <iostream>
using namespace std;

int main() {
  return 0;
}
```
**Makefile**
```Makefile
main: main.cpp
	@g++ main.cpp
	@./a.out
```
