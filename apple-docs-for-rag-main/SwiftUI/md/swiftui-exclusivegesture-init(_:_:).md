

- SwiftUI
- ExclusiveGesture
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Creates a gesture from two gestures where only one of them succeeds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    _ first: First,
    _ second: Second
)
```

## Parameters 

`first`  

The first of two gestures. This gesture has precedence over the other gesture.

`second`  

The second of two gestures.

## See Also

### Creating the gesture

var first: First

The first of two gestures.

var second: Second

The second of two gestures.

