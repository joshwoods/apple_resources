

- SwiftUI
- UIGestureRecognizerRepresentable
-  makeUIGestureRecognizer(context:) 

Instance Method

# makeUIGestureRecognizer(context:)

Creates an instance of the represented gesture recognizer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func makeUIGestureRecognizer(context: Self.Context) -> Self.UIGestureRecognizerType
```

**Required**

## Parameters 

`context`  

A context structure containing information about the current state of the system, such as the current coordinator instance.

## Discussion

Note

Gesture recognizers are created on-demand and torn down when an event sequence ends, so do not perform expensive work in this method.

