

- SwiftUI
- Gesture
-  sequenced(before:) 

Instance Method

# sequenced(before:)

Sequences a gesture with another one to create a new gesture, which results in the second gesture only receiving events after the first gesture succeeds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func sequenced(before other: Other) -> SequenceGesture where Other : Gesture
```

## Parameters 

`other`  

A gesture you want to combine with another gesture to create a new, sequenced gesture.

## Return Value

A gesture that’s a sequence of two gestures.

## See Also

### Composing gestures

func simultaneously&lt;Other>(with: Other) -> SimultaneousGesture&lt;Self, Other>

Combines a gesture with another gesture to create a new gesture that recognizes both gestures at the same time.

func exclusively&lt;Other>(before: Other) -> ExclusiveGesture&lt;Self, Other>

Combines two gestures exclusively to create a new gesture where only one gesture succeeds, giving precedence to the first gesture.

