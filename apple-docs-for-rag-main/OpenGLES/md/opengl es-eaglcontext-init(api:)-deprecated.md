

- OpenGL ES
- EAGLContext
-  init(api:) Deprecated

Initializer

# init(api:)

Initializes and returns a newly allocated rendering context with the specified version of the OpenGL ES rendering API.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
convenience init?(api: EAGLRenderingAPI)
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`api`  

The desired version of the OpenGL ES rendering API. For legal values, see EAGLRenderingAPI.

## Return Value

An initialized context object, or `nil` if the object couldn’t be created.

## Discussion

To issue OpenGL ES commands to this context, you must first make the context current by calling setCurrent(_:).

Calling init(api:) creates a new EAGLSharegroup object and attaches it to this context.

## See Also

### Related Documentation

OpenGL ES Programming Guide

