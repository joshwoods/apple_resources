

- OpenGL ES
- EAGLDrawable
-  drawableProperties Deprecated

Instance Property

# drawableProperties

A dictionary of values that specify the desired characteristics of the drawable surface.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
var drawableProperties: [String : Any]? { get set }
```

**Required**

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The `drawableProperties` dictionary specifies the properties that are used by this object when it is attached to an OpenGL ES renderbuffer. Your application should set these properties before passing this object into the `EAGLContext` method renderbufferStorage(_:from:). If you change the `drawableProperties` dictionary, your application must call renderbufferStorage(_:from:) again on the context for the new values to take effect.

## See Also

### Related Documentation

OpenGL ES Programming Guide

