

- OpenGL ES
- EAGLContext
-  sharegroup Deprecated

Instance Property

# sharegroup

The context’s sharegroup object. (read-only)

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
var sharegroup: EAGLSharegroup { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

Retrieve the sharegroup of a context when you want to create two or more contexts that share rendering resources. Call init(api:) to initialize the first context, retrieve its sharegroup, and then initialize additional contexts by calling init(api:sharegroup:), passing this sharegroup as the parameter.

## See Also

### Related Documentation

init?(api: EAGLRenderingAPI, sharegroup: EAGLSharegroup)

Initializes and returns a newly allocated rendering context with the specified version of OpenGL ES rendering API and the specified sharegroup.

Deprecated

