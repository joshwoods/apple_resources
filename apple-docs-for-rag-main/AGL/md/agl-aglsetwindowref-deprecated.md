

- AGL
-  aglSetWindowRef Deprecated

Function

# aglSetWindowRef

Sets an AGL context to the specified window.

macOS 10.5–10.9Deprecated

``` source
extern GLboolean aglSetWindowRef(AGLContext ctx, WindowRef window);
```

## Parameters 

`ctx`  

An AGL context.

`window`  

The window to set.

## Return Value

`true` if the window is successfully set; `false` otherwise.

## See Also

### Getting and Setting Windows

aglGetWindowRef

Retrieves the window associated with an AGL context.

