
## SDL2 OpenGL Basic Template

Simple and useful (supposedly) cross-platform template for OpenGL. Uses SDL_GL_GetProcAddress() to create the OpenGL functions so that you do not need to link or include the OS specific opengl library. 



```C++
// Use this!
#include <opengl.h>
// instead of
#include <gl.h>
// or
#include <SDL2/SDL_opengl.h>
```

..and you don't need to link it in the Makefile..

```Makefile
LDLIBS = -lSDL2 # No gl here
```


## Credits

The [opengl.h](opengl.h) and [opengl.cpp](opengl.cpp) files are by nlguillemot who provided the source code and explains code in [this article](https://nlguillemot.wordpress.com/2016/11/18/opengl-renderer-design/). The code is also derived from from Khronos' glcorearb.h. 