

- Network Extension
- NWPath
-  status Deprecated

Instance Property

# status

The evaluated status of the network path.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var status: NWPathStatus { get }
```

Deprecated

Use the nw_path_get_status(_:) function from the Network framework instead.

## Discussion

The status of a path indicates whether or not the process is able to make connection attempts to any, or a specific, network endpoint. A satisfied status does not guarantee that a connection will be successful, but it does ensure that there is some interface over which an attempt can be made.

## See Also

### Getting network path properties

enum NWPathStatusDeprecated

var isExpensive: Bool

A Boolean that indicates whether or not the path uses an expensive interface.

Deprecated

var isConstrained: Bool

A Boolean that indicates whether or not the path uses a constrained interface, such as when using low-data mode.

Deprecated

