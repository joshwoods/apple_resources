

- Network Extension
- NEFilterProviderConfiguration
-  filterBrowsers 

Instance Property

# filterBrowsers

A Boolean value that indicates that the system applies the filter to flows of network data originated from WebKit browser objects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11–10.15DeprecatedvisionOS 1.0+

``` source
var filterBrowsers: Bool { get set }
```

## Discussion

The default value of this property is false.

## See Also

### Configuring filter behavior

var filterSockets: Bool

A Boolean value that indicates that the system applies the filter to flows of network data originated from sockets.

var filterPackets: Bool

A Boolean value that indicates that the system applies the filter to packets of network data.

