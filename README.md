# SIMPLE-Graphic
Rendering engine for all SIMPLE projects that require graphics rendering
## Usage
1. Clone SIMPLE-Graphic to local:
```bash
git clone https://github.com/Tianxiaoxiao1021/SIMPLE-Graphic (local path)
```
### tips
If there are any SIMPLE projects that require local graphics rendering, clone SIMPLE-Graphic to the path:
../path/to/lib/SIMPLE-xxx/dependency/SIMPLE-Graphics(always empty)

2. If you haven't local SIMPLE project require the graphics rendering, you can use it in your code:
example:
```cpp
#include "../SIMPLE-Graphics/Engine.h"
using namespace std;
int main(){
  SrenderEngine engine;
  engine.init();
  while(true){
    engine.update();
    engine.render();
    engine.clearbuffer();
  }
  return 0;
}
```
## tips
make sure your C++ complier supports C++14 and above, the SIMPLE-Graphics used very lots of morden C++'s features.
