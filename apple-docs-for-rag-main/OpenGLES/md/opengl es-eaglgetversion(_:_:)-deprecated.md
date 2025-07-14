

- OpenGL ES
-  EAGLGetVersion(\_:\_:) Deprecated

Function

# EAGLGetVersion(\_:\_:)

Retrieves the version information for the EAGL implementation.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func EAGLGetVersion(
    _ major: UnsafeMutablePointer,
    _ minor: UnsafeMutablePointer
)
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`major`  

On output, the major version of the EAGL implementation.

`minor`  

On output, the minor version of the EAGL implementation.

## Discussion

If `major` and `minor` parameters are not `nil`, they return the major and minor version number of the EAGL implementation, respectively.

