

- Core Bluetooth
-  CBManagerAuthorization 

Enumeration

# CBManagerAuthorization

The current authorization state of a Core Bluetooth manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum CBManagerAuthorization
```

## Topics

### Authorization States

case allowedAlways

A state that indicates the user has authorized Bluetooth at any time.

case denied

A state that indicates the user explicitly denied Bluetooth access for this app.

case notDetermined

A state that indicates the user has yet to authorize Bluetooth for this app.

case restricted

A state that indicates this app isn’t authorized to use Bluetooth.

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

### Determining Authorization State

class var authorization: CBManagerAuthorization

The current authorization status for using Bluetooth.

