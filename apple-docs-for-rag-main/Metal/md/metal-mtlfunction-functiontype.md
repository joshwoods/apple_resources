

- Metal
- MTLFunction
-  functionType 

Instance Property

# functionType

The shader function’s type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var functionType: MTLFunctionType { get }
```

**Required**

## Discussion

A function’s type determines what kind of pipeline state objects you can create from it and whether you can use it as a callable function in a function table.

## See Also

### Identifying Shader Functions

var device: any MTLDevice

The device object that created the shader function.

**Required**

var label: String?

A string that identifies the shader function.

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

