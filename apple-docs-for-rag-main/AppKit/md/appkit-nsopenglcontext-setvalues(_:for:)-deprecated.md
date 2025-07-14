

- AppKit
- NSOpenGLContext
-  setValues(\_:for:) Deprecated

Instance Method

# setValues(\_:for:)

Sets the value of the specified parameter.

macOS 10.0–10.14Deprecated

``` source
func setValues(
    _ vals: UnsafePointer,
    for param: NSOpenGLContext.Parameter
)
```

Deprecated

Please use Metal or MetalKit.

## Parameters 

`vals`  

The new value (or values) for the parameter.

`param`  

The parameter you want to modify. For a list of parameters, see NSOpenGLContext.Parameter.

## See Also

### Context Parameter Handling

func getValues(UnsafeMutablePointer&lt;GLint>, for: NSOpenGLContext.Parameter)

Returns the value of the requested parameter.

Deprecated

