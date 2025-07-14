

- UIKit
-  UIPointerRegionRequest 

Class

# UIPointerRegionRequest

An object to describe the pointer’s location in the interaction’s view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class UIPointerRegionRequest
```

## Overview

The `UIPointerRegionRequest` is given to the `UIPointerInteractionDelegate` to allow for changes to the pointer interaction.

## Topics

### Inspecting the region request

var location: CGPoint

The location of the pointer in the interaction’s view’s coordinate space.

var modifiers: UIKeyModifierFlags

Key modifier flags representing keyboard keys pressed by the user at the time of this request.

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

### Pointer region

class UIPointerRegion

A rectangular region that interacts with pointer movements.

