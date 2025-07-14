

- Network Extension
- NEFilterProviderConfiguration
-  filterSockets 

Instance Property

# filterSockets

A Boolean value that indicates that the system applies the filter to flows of network data originated from sockets.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var filterSockets: Bool { get set }
```

## Discussion

The default value of this property is false.

## See Also

### Configuring filter behavior

var filterBrowsers: Bool

A Boolean value that indicates that the system applies the filter to flows of network data originated from WebKit browser objects.

var filterPackets: Bool

A Boolean value that indicates that the system applies the filter to packets of network data.

