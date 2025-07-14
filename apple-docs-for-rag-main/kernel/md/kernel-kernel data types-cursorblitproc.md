

- Kernel
- Kernel Data Types
-  CursorBlitProc 

Type Alias

# CursorBlitProc

macOS 10.0+

``` source
typedef void (*CursorBlitProc)(IOFramebuffer *inst, void *shmem, volatile unsigned char *vramPtr, unsigned int cursStart, unsigned int vramRow, unsigned int cursRow, int width, int height);
```

