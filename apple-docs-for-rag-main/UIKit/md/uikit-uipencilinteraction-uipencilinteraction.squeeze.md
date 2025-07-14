

- UIKit
- UIPencilInteraction
-  UIPencilInteraction.Squeeze 

Class

# UIPencilInteraction.Squeeze

An interaction that represents a squeeze on Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
class Squeeze
```

## Topics

### Getting information about a squeeze interaction

var timestamp: TimeInterval

The timestamp of the squeeze interaction.

var phase: UIPencilInteraction.Phase

The phase of a squeeze interaction on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

var hoverPose: UIPencilHoverPose?

The hover pose of Apple Pencil during a squeeze interaction.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

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
- Sendable

## See Also

### Apple Pencil interactions in UIKit

class UIPencilInteraction

An interaction that tells your app when a person double-taps or squeezes Apple Pencil.

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

class Tap

An interaction that represents a double tap on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

