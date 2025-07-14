

- Virtualization
- VZMacHardwareModel
-  dataRepresentation 

Instance Property

# dataRepresentation

Returns the opaque data representation of the hardware model.

macOS 12.0+

``` source
var dataRepresentation: Data { get }
```

## Discussion

You can use this to recreate the same hardware model with init(dataRepresentation:).

## See Also

### Configuring the hardware model

var isSupported: Bool

A Boolean value that indicates whether the host supports this hardware model.

