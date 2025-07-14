

- MapKit
- MKAnnotationView
-  MKAnnotationView.DragState 

Enumeration

# MKAnnotationView.DragState

Constants that indicate the drag state of an annotation view.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
enum DragState
```

## Topics

### Constants

case none

An annotation view that doesn’t have a drag operation.

case starting

An annotation view begins dragging.

case dragging

An annotation view is actively dragging.

case canceling

An annotation view cancels drag operation.

case ending

An annotation view ends dragging.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

