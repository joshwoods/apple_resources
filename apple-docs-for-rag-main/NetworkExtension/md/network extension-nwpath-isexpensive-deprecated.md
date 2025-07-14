

- Network Extension
- NWPath
-  isExpensive Deprecated

Instance Property

# isExpensive

A Boolean that indicates whether or not the path uses an expensive interface.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var isExpensive: Bool { get }
```

Deprecated

Use the nw_path_is_expensive(_:) function from the Network framework instead.

## Discussion

Returns YES is the path uses an interface that is considered expensive, such as when using a cellular data plan.

## See Also

### Getting network path properties

var status: NWPathStatus

The evaluated status of the network path.

Deprecated

enum NWPathStatusDeprecated

var isConstrained: Bool

A Boolean that indicates whether or not the path uses a constrained interface, such as when using low-data mode.

Deprecated

