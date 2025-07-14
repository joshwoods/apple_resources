

- AppKit
- NSOpenGLContext
-  getValues(\_:for:) Deprecated

Instance Method

# getValues(\_:for:)

Returns the value of the requested parameter.

macOS 10.0–10.14Deprecated

``` source
func getValues(
    _ vals: UnsafeMutablePointer,
    for param: NSOpenGLContext.Parameter
)
```

Deprecated

Please use Metal or MetalKit.

## Parameters 

`vals`  

On input, a pointer to a variable with enough space for one or more `long` integers. On output, the variable contains the value (or values) for the given parameter.

`param`  

The parameter you want to get. For a list of parameters, see the table in NSOpenGLContext.Parameter.

## See Also

### Context Parameter Handling

func setValues(UnsafePointer&lt;GLint>, for: NSOpenGLContext.Parameter)

Sets the value of the specified parameter.

Deprecated

