

- Network
- NWPath
-  NWPath.Status 

Enumeration

# NWPath.Status

Status values indicating whether a path can be used by connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum Status
```

## Topics

### Status Values

case unsatisfied

The path is not available for use.

case satisfied

The path is available to establish connections and send data.

case requiresConnection

The path is not currently available, but establishing a new connection may activate the path.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Checking Path Availability

let status: NWPath.Status

A status indicating whether a path can be used by connections.

