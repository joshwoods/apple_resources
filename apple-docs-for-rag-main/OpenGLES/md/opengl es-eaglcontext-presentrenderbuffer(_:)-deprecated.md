

- OpenGL ES
- EAGLContext
-  presentRenderbuffer(\_:) Deprecated

Instance Method

# presentRenderbuffer(\_:)

Displays a renderbuffer’s contents on screen.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func presentRenderbuffer(_ target: Int) -> Bool
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`target`  

The OpenGL ES binding point for a currently bound renderbuffer. The value of this parameter must be `GL_RENDERBUFFER` (or `GL_RENDERBUFFER_OES` in an OpenGL ES 1.1 context).

## Return Value

true if successful; otherwise, false.

## Discussion

The renderbuffer to be displayed must have been allocated storage using the renderbufferStorage(_:from:) method. The exact semantics for how and when the renderbuffer contents are displayed is controlled by the drawable object.

Important

The contents of the renderbuffer may be altered after the renderbuffer is presented to the screen. After presenting the renderbuffer, your application must *completely* redraw the contents of the renderbuffer before presenting it again. To preserve the contents of the renderbuffer you may set the kEAGLDrawablePropertyRetainedBacking key of the `drawableProperties` dictionary to true. Setting the key to true may result in reduced graphics performance and increased memory usage. Therefore, choose this setting only when you need the renderbuffer’s contents to remain unchanged.

## See Also

### Related Documentation

func renderbufferStorage(Int, from: (any EAGLDrawable)?) -> Bool

Binds a drawable object’s storage to an OpenGL ES renderbuffer object.

Deprecated

