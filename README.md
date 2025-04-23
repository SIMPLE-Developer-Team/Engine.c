# SIMPLE-Graphic
A simple, cross-platfrom and single-file graphics rendering engine for C/C++.
## requirements
- C version: C98+
- C++ version: C++11+
- OpenGL version: 3.0+
## example:
```c
#include "Engine.h"
int main(){
  SrenderEngine engine;
  Sstatus initstatus;
  initstatus = initEngine(&engine);
  if(initstatus == Sfail){
    printf("Failed to init engine!\n");
    return -1;
  }
  initstatus = initWindow(&engine, 800, 600, "Test window", Sfalse);
  if(initstatus == Sfail){
    printf("Failed to create window!\n");
    return -1;
  }
  Vertex v[] = {
    {{0,0}, WHITE},
    {{0, 600}, WHITE},
    {{800, 600}, WHITE}
  };
  unsigned int index[] = {0, 1, 2};
  setVertexData(&engine, v, 3);
  setIndexData(&engine, index, 3);
  while(!shouldclose(&engine)){
    render_and_update(&engine);
  }
  freeEngine(&engine);
  return 0;
}
```
Code will create a 800*600's window with a triangle , the title will be "Test window".
