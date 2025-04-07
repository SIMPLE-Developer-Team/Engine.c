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
int main(){
  SrenderEngine engine;
  initengine(&engine);
  setupwindow(&engine, 800, 600, "Test window");
  while(true){
    update(&engine);
  }
  return 0;
}
```
Code will create a 800*600's window, the title will be "Test window".
