# SIMPLE-Graphic
A simple cross-platfrom graphics rendering engine for C/C++, based on OpenGL/GLFW
## Usage
1. Clone SIMPLE-Graphic to local:
```bash
git clone https://github.com/Tianxiaoxiao1021/SIMPLE-Graphic (local path)
```
2. Add GLFW path to your project.
  
This is a example for use this engine.
```c
#include "../SIMPLE-Graphics/Engine.h"
using namespace std;
int main(){
  SrenderEngine engine;
  engine.init();
  engine.setupwindow(800, 600, "Test Window");
  while(true){
    engine.update();
  }
  return 0;
}
```
Code will create a 800*600's window, the title will be "Test window".
