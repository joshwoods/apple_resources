

- OpenGL ES
-  kEAGLDrawablePropertyRetainedBacking Deprecated

Global Variable

# kEAGLDrawablePropertyRetainedBacking

The key specifying whether the drawable surface retains its contents after displaying them. The value for this key is an `NSNumber` object containing a `BOOL` data type. If `false`, you may not rely on the contents being the same after the contents are displayed. If `true`, then the contents will not change after being displayed. Setting the value to `true` is recommended only when you need the content to remain unchanged, as using it can result in both reduced performance and additional memory usage. The default value is `false`.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
let kEAGLDrawablePropertyRetainedBacking: String
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

