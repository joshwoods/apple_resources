

- Metal
- MTLFunction
-  device 

Instance Property

# device

The device object that created the shader function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

You can only use this function object with this MTLDevice.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Identifying Shader Functions

var label: String?

A string that identifies the shader function.

**Required**

var functionType: MTLFunctionType

The shader function’s type.

**Required**

var name: String

The function’s name.

**Required**

enum MTLFunctionType

The type of a top-level Metal Shading Language (MSL) function.

var options: MTLFunctionOptions

The options that Metal used to compile this function.

**Required**

struct MTLFunctionOptions

Options that define how Metal creates the function object.

