

- UIKit
- UIPressesEvent
-  allPresses 

Instance Property

# allPresses

The state of all physical buttons in the event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var allPresses: Set { get }
```

## Return Value

The set of UIPress instances that participated in this event.

## See Also

### Reading the event button presses

func presses(for: UIGestureRecognizer) -> Set&lt;UIPress>

Returns the state of all physical buttons in the event that are associated with a particular gesture recognizer.

