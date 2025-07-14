

- UIKit
- UIPressesEvent
-  presses(for:) 

Instance Method

# presses(for:)

Returns the state of all physical buttons in the event that are associated with a particular gesture recognizer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func presses(for gesture: UIGestureRecognizer) -> Set
```

## Parameters 

`gesture`  

A gesture recognizer.

## Return Value

The set of UIPress instances that participated in this event that are associated with the gesture recognizer.

## See Also

### Reading the event button presses

var allPresses: Set&lt;UIPress>

The state of all physical buttons in the event.

