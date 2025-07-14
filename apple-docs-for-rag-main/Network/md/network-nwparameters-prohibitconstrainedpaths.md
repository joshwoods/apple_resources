

- Network
- NWParameters
-  prohibitConstrainedPaths 

Instance Property

# prohibitConstrainedPaths

A Boolean that prevents connections, listeners, and browsers from using network paths marked as constrained by Low Data Mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final var prohibitConstrainedPaths: Bool { get set }
```

## See Also

### Selecting Paths

var requiredInterfaceType: NWInterface.InterfaceType

An interface type to require on connections and listeners.

var requiredInterface: NWInterface?

A specific interface to require on connections, listeners, and browsers.

var requiredLocalEndpoint: NWEndpoint?

A specific local IP address and port to use for connections and listeners.

var prohibitExpensivePaths: Bool

A Boolean that prevents connections, listeners, and browsers from using network paths marked as expensive.

var prohibitedInterfaceTypes: [NWInterface.InterfaceType]?

A list of interface types that connections, listeners, and browsers will not use.

var prohibitedInterfaces: [NWInterface]?

A list of specific interfaces that connections and listeners will not use.

