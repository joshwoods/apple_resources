

- Virtualization
- VZMacMachineIdentifier
-  dataRepresentation 

Instance Property

# dataRepresentation

Returns the opaque data representation of the machine identifier.

macOS 12.0+

``` source
var dataRepresentation: Data { get }
```

## Discussion

You can use this to recreate the same machine identifier with init(dataRepresentation:).

