

- Network Extension
-  NWPath Deprecated

Class

# NWPath

The path made by a network connection, including information about its viability.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWPath
```

Deprecated

Use the nw_path_t type from the Network framework instead.

## Overview

For example, if the path status is NWPathStatus.satisfied, then a connection attempt will be made.

When attached to a specific connection, a path takes all of the connection parameters into account. For example, if the route for a connection changes or is removed, the path will reflect that change. Note that every path is evaluated within the context of the process it is running in, and may be different across processes.

NWPath is a static object, and properties of the path will never change. To monitor changing network status, use Key-Value Observing (KVO) to watch a path property on another object. For information about KVO, see Key-Value Observing Programming Guide.

## Topics

### Getting network path properties

var status: NWPathStatus

The evaluated status of the network path.

enum NWPathStatus

var isExpensive: Bool

A Boolean that indicates whether or not the path uses an expensive interface.

var isConstrained: Bool

A Boolean that indicates whether or not the path uses a constrained interface, such as when using low-data mode.

### Comparing network paths

func isEqual(to: NWPath) -> Bool

Comparison method for NWPath objects.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

