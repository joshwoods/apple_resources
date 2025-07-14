

- SwiftUI
- UIGestureRecognizerRepresentable
-  makeCoordinator(converter:) 

Instance Method

# makeCoordinator(converter:)

Creates the custom object that you use to communicate state changes from your gesture recognizer to other parts of your SwiftUI interface.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func makeCoordinator(converter: Self.CoordinateSpaceConverter) -> Self.Coordinator
```

**Required** Default implementation provided.

## Parameters 

`converter`  

A structure used to convert locations to/from coordinate spaces in the hierarchy of the associated SwiftUI view.

## Discussion

You access the resulting coordinator via the `Context` passed into other methods in this protocol.

## Default Implementations

### UIGestureRecognizerRepresentable Implementations

func makeCoordinator(converter: Self.CoordinateSpaceConverter)

