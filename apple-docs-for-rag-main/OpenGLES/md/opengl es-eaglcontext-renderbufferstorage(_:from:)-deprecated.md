

- OpenGL ES
- EAGLContext
-  renderbufferStorage(\_:from:) Deprecated

Instance Method

# renderbufferStorage(\_:from:)

Binds a drawable object’s storage to an OpenGL ES renderbuffer object.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func renderbufferStorage(
    _ target: Int,
    from drawable: (any EAGLDrawable)?
) -> Bool
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`target`  

The OpenGL ES binding point for a currently bound renderbuffer. The value of this parameter must be `GL_RENDERBUFFER` (or `GL_RENDERBUFFER_OES` in an OpenGL ES 1.1 context).

`drawable`  

An object managing the data store for the renderbuffer. In iOS, the value of this parameter must be a CAEAGLLayer object.

## Return Value

true if successful; otherwise, false.

## Discussion

To create a renderbuffer that can be presented to the screen, you bind the renderbuffer and then allocate shared storage for it by calling this method. This method call replaces the call normally made to `glRenderbufferStorage`. A renderbuffer whose storage has been allocated with this method can later be displayed with a call to presentRenderbuffer(_:).

The width, height, and internal color buffer format are derived from the characteristics of the drawable object. You may override the internal color buffer format by adding an kEAGLDrawablePropertyColorFormat key to the drawableProperties dictionary of the drawable object before calling this method.

To specify that the OpenGL ES renderbuffer should be detached from the drawable object, call this method with the `drawable` parameter set to `nil`.

### Special Considerations

In iOS 6.0 and later, this method automatically flushes the OpenGL ES command buffer, making it unsuitable to call repeatedly in performance-critical code.

