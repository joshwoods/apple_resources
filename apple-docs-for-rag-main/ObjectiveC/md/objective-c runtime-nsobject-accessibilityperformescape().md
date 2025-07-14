

- Objective-C Runtime
- NSObject
-  accessibilityPerformEscape() 

Instance Method

# accessibilityPerformEscape()

Dismisses a modal view and returns the success or failure of the action.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityPerformEscape() -> Bool
```

## Return Value

YES if the modal view is successfully dismissed; otherwise, NO. By default, this method returns NO.

## Discussion

Implement this method on an element or containing view that can be revealed modally or in a hierarchy. When a VoiceOver user performs a dismiss action, this method dismisses the view. For example, you might implement this method for a popover in order to give users a deliberate dismiss action to perform that closes the popover.

## See Also

### Performing an action

func accessibilityActivate() -> Bool

Tells the element to activate itself and report the success or failure of the operation.

func accessibilityIncrement()

Tells the accessibility element to increment the value of its content.

func accessibilityDecrement()

Tells the accessibility element to decrement the value of its content.

func accessibilityScroll(UIAccessibilityScrollDirection) -> Bool

Scrolls screen content in an application-specific way and returns the success or failure of the action.

func accessibilityPerformMagicTap() -> Bool

Performs a salient action.

