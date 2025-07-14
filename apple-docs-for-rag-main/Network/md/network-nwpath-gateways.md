

- Network
- NWPath
-  gateways 

Instance Property

# gateways

A list of gateways configured on the interfaces available to a path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var gateways: [NWEndpoint] { get }
```

## See Also

### Inspecting Interfaces

func usesInterfaceType(NWInterface.InterfaceType) -> Bool

Checks if connections using the path may send traffic over a specific interface type.

let availableInterfaces: [NWInterface]

A list of all interfaces available to the path, in order of preference.

