

- Core Motion
- CMHeadphoneActivityManager
-  CMHeadphoneActivityManager.Status 

Enumeration

# CMHeadphoneActivityManager.Status

Headphone connection status updates.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+watchOS 2.0+

``` source
enum Status
```

## Topics

### Enumeration Cases

case connected

A compatible set of headphones is connected.

case disconnected

The headphones disconnected.

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

### Supporting Types

typealias ActivityHandler

The type for a handler to be invoked when headphone motion activity data is available.

typealias StatusHandler

The type for a handler to be invoked with status updates.

