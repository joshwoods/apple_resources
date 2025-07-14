

- Metal
- MTLFunctionHandle
-  device 

Instance Property

# device

The device object that created the shader function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

You can only use the function handle with this MTLDevice.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Querying Handle Properties

var functionType: MTLFunctionType

The shader function’s type.

**Required**

var name: String

The function’s name.

**Required**

