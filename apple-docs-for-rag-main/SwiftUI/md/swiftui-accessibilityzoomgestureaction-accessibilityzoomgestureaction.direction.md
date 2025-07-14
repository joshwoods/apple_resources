

- SwiftUI
- AccessibilityZoomGestureAction
-  AccessibilityZoomGestureAction.Direction 

Enumeration

# AccessibilityZoomGestureAction.Direction

A direction that matches the movement of a zoom gesture performed by an assistive technology, such as a swipe up and down in Voiceover’s zoom rotor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum Direction
```

## Topics

### Getting the direction

case zoomIn

The gesture direction that represents zooming in.

case zoomOut

The gesture direction that represents zooming out.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the action’s direction

let direction: AccessibilityZoomGestureAction.Direction

The zoom gesture’s direction.

