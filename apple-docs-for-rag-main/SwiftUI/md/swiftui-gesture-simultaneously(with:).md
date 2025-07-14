

- SwiftUI
- Gesture
-  simultaneously(with:) 

Instance Method

# simultaneously(with:)

Combines a gesture with another gesture to create a new gesture that recognizes both gestures at the same time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func simultaneously(with other: Other) -> SimultaneousGesture where Other : Gesture
```

## Parameters 

`other`  

A gesture that you want to combine with your gesture to create a new, combined gesture.

## Return Value

A gesture with two simultaneous gestures.

## See Also

### Composing gestures

func sequenced&lt;Other>(before: Other) -> SequenceGesture&lt;Self, Other>

Sequences a gesture with another one to create a new gesture, which results in the second gesture only receiving events after the first gesture succeeds.

func exclusively&lt;Other>(before: Other) -> ExclusiveGesture&lt;Self, Other>

Combines two gestures exclusively to create a new gesture where only one gesture succeeds, giving precedence to the first gesture.

