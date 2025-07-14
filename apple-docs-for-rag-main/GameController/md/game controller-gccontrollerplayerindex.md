

- Game Controller
-  GCControllerPlayerIndex 

Enumeration

# GCControllerPlayerIndex

The possible values for controller player indices.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
enum GCControllerPlayerIndex
```

## Topics

### Player indices

case indexUnset

The default index for a player on a controller.

case index1

Player one is using the controller.

case index2

Player two is using the controller.

case index3

Player three is using the controller.

case index4

Player four is using the controller.

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

### Identifying controllers and displaying a player index

var playerIndex: GCControllerPlayerIndex

The player index for the controller.

