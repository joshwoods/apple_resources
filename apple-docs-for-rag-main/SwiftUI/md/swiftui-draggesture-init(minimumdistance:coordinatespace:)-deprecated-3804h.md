

- SwiftUI
- DragGesture
-  init(minimumDistance:coordinateSpace:) Deprecated

Initializer

# init(minimumDistance:coordinateSpace:)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
@MainActor @preconcurrency
init(
    minimumDistance: CGFloat = 10,
    coordinateSpace: CoordinateSpace = .local
)
```

Deprecated

Use init(minimumDistance:coordinateSpace:) instead.

Show all declarations

## Parameters 

`minimumDistance`  

The minimum dragging distance for the gesture to succeed.

`coordinateSpace`  

The coordinate space of the dragging gesture’s location.

