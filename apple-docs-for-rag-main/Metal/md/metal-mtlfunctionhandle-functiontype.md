

- Metal
- MTLFunctionHandle
-  functionType 

Instance Property

# functionType

The shader function’s type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var functionType: MTLFunctionType { get }
```

**Required**

## Discussion

A function’s type determines what kind of pipeline state objects you can create from it.

## See Also

### Querying Handle Properties

var device: any MTLDevice

The device object that created the shader function.

**Required**

var name: String

The function’s name.

**Required**

