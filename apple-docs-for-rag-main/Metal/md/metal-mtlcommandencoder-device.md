

- Metal
- MTLCommandEncoder
-  device 

Instance Property

# device

The Metal device from which the command encoder was created.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

This command encoder can only be used with this MTLDevice.

## See Also

### Identifying the Command Encoder

var label: String?

A string that labels the command encoder.

**Required**

