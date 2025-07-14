

- OpenGL ES
- EAGLContext
-  debugLabel Deprecated

Instance Property

# debugLabel

A label describing the context for use in debugging.

iOS 6.0–12.0DeprecatediPadOS 6.0–12.0DeprecatedMac Catalyst 6.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
var debugLabel: String? { get set }
```

## Discussion

Use this property to provide a meaningful name for a context. This label, which appears in the Xcode OpenGL ES Frame Debugger interface, makes it easy for you to more easily keep track of different contexts when debugging a multicontext app.

