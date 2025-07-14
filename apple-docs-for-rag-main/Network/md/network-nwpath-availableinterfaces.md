

- Network
- NWPath
-  availableInterfaces 

Instance Property

# availableInterfaces

A list of all interfaces available to the path, in order of preference.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
let availableInterfaces: [NWInterface]
```

## See Also

### Inspecting Interfaces

func usesInterfaceType(NWInterface.InterfaceType) -> Bool

Checks if connections using the path may send traffic over a specific interface type.

var gateways: [NWEndpoint]

A list of gateways configured on the interfaces available to a path.

