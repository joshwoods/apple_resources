

- UIKit
- UIPencilInteraction
-  UIPencilInteraction.Phase 

Enumeration

# UIPencilInteraction.Phase

Constants that describe the phases of an interaction on Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
enum Phase
```

## Topics

### Phases

case began

case cancelled

case changed

case ended

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Apple Pencil interactions in UIKit

class UIPencilInteraction

An interaction that tells your app when a person double-taps or squeezes Apple Pencil.

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

class Tap

An interaction that represents a double tap on Apple Pencil.

class Squeeze

An interaction that represents a squeeze on Apple Pencil.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

