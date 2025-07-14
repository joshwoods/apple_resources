

- SwiftUI
- DragGesture
-  init(minimumDistance:coordinateSpace:) 

Initializer

# init(minimumDistance:coordinateSpace:)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    minimumDistance: CGFloat = 10,
    coordinateSpace: some CoordinateSpaceProtocol = .local
)
```

Show all declarations

## Parameters 

`minimumDistance`  

The minimum dragging distance for the gesture to succeed.

`coordinateSpace`  

The coordinate space of the dragging gesture’s location.

