

- OpenGL ES
- EAGLContext
-  init(api:sharegroup:) Deprecated

Initializer

# init(api:sharegroup:)

Initializes and returns a newly allocated rendering context with the specified version of OpenGL ES rendering API and the specified sharegroup.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
init?(
    api: EAGLRenderingAPI,
    sharegroup: EAGLSharegroup
)
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`api`  

The desired version of the OpenGL ES rendering API. For legal values, see EAGLRenderingAPI.

`sharegroup`  

A sharegroup obtained from another EAGLContext object.

## Return Value

An initialized context object, or `nil` if the object couldn’t be created.

## Discussion

To issue OpenGL ES commands to this context, you must first make it the current drawing context by calling setCurrent(_:).

OpenGL ES objects such as textures, renderbuffers, framebuffers and vertex buffers are shared across all contexts that are created with the same sharegroup. To specify that a new context should be initialized in an existing sharegroup, retrieve the sharegroup property from a previously initialized context and pass it as a parameter to this initialization method. Pass `nil` as the `sharegroup` parameter to create a new EAGLSharegroup object attached to the context.

