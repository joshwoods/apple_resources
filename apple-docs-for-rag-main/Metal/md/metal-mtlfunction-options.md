

- Metal
- MTLFunction
-  options 

Instance Property

# options

The options that Metal used to compile this function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var options: MTLFunctionOptions { get }
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

var name: String

The function’s name.

**Required**

enum MTLFunctionType

The type of a top-level Metal Shading Language (MSL) function.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

