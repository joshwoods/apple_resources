

- SwiftUI
- Gesture
-  exclusively(before:) 

Instance Method

# exclusively(before:)

Combines two gestures exclusively to create a new gesture where only one gesture succeeds, giving precedence to the first gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func exclusively(before other: Other) -> ExclusiveGesture where Other : Gesture
```

## Parameters 

`other`  

A gesture you combine with your gesture, to create a new, combined gesture.

## Return Value

A gesture that’s the result of combining two gestures where only one of them can succeed. SwiftUI gives precedence to the first gesture.

## See Also

### Composing gestures

func simultaneously&lt;Other>(with: Other) -> SimultaneousGesture&lt;Self, Other>

Combines a gesture with another gesture to create a new gesture that recognizes both gestures at the same time.

func sequenced&lt;Other>(before: Other) -> SequenceGesture&lt;Self, Other>

Sequences a gesture with another one to create a new gesture, which results in the second gesture only receiving events after the first gesture succeeds.

