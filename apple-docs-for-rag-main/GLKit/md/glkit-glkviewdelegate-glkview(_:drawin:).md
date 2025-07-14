

- GLKit
- GLKViewDelegate
-  glkView(\_:drawIn:) 

Instance Method

# glkView(\_:drawIn:)

Draws the view’s contents.

iOS 5.0+iPadOS 5.0+tvOS 9.0+

``` source
func glkView(
    _ view: GLKView,
    drawIn rect: CGRect
)
```

**Required**

## Parameters 

`view`  

The view requesting that its contents be redrawn.

`rect`  

A rectangle that describes the area that needs to be updated.

## Discussion

The semantics of this method are identical to those of the draw(_:) method; the GLKView object makes its OpenGL ES context the current context and binds its framebuffer as the target for OpenGL ES rendering commands. Your delegate method should then draw the view’s contents.

