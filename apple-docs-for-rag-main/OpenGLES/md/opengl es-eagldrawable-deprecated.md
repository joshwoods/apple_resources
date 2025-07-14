

- OpenGL ES
-  EAGLDrawable Deprecated

Protocol

# EAGLDrawable

iOS objects that implement the `EAGLDrawable` protocol can be used as a rendering surface and displayed to the screen by an `EAGLContext` object. In iOS 2.0, this protocol is implemented only by the `CAEAGLLayer` class, but in the future other classes may choose to implement the protocol. The `EAGLDrawable` protocol is not intended to be implemented by objects outside of the iOS.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
protocol EAGLDrawable
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Topics

### Drawable Properties

var drawableProperties: [String : Any]?

A dictionary of values that specify the desired characteristics of the drawable surface.

**Required**

### Constants

Drawable Property Keys

Keys to specify in the `drawableProperties` dictionary.

Color Formats

Color formats that can be specified under the `kEAGLDrawablePropertyColorFormat` key.

