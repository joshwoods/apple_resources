

- Network Extension
-  NWPathStatus Deprecated

Enumeration

# NWPathStatus

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
enum NWPathStatus
```

Deprecated

Use the nw_path_status_t type from the Network framework instead.

## Topics

### Path Statuses

case invalid

The path cannot be evaluated.

case satisfied

The path is ready to be used for network connections.

case unsatisfied

The path for network connections is not available, either due to lack of network connectivity or being prohibited by system policy.

case satisfiable

The path is not currently satisfied, but may become satisfied upon a connection attempt. This can be due to a service, such as a VPN or a cellular data connection not being activated.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting network path properties

var status: NWPathStatus

The evaluated status of the network path.

Deprecated

var isExpensive: Bool

A Boolean that indicates whether or not the path uses an expensive interface.

Deprecated

var isConstrained: Bool

A Boolean that indicates whether or not the path uses a constrained interface, such as when using low-data mode.

Deprecated

