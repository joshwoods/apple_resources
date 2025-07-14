

- Metal
- MTLFunction
-  name 

Instance Property

# name

The function’s name.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var name: String { get }
```

**Required**

## See Also

### Identifying Shader Functions

var device: any MTLDevice

The device object that created the shader function.

**Required**

var label: String?

A string that identifies the shader function.

**Required**

var functionType: MTLFunctionType

The shader function’s type.

**Required**

enum MTLFunctionType

The type of a top-level Metal Shading Language (MSL) function.

var options: MTLFunctionOptions

The options that Metal used to compile this function.

**Required**

struct MTLFunctionOptions

Options that define how Metal creates the function object.

