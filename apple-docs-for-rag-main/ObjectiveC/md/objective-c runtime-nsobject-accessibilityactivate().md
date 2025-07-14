

- Objective-C Runtime
- NSObject
-  accessibilityActivate() 

Instance Method

# accessibilityActivate()

Tells the element to activate itself and report the success or failure of the operation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityActivate() -> Bool
```

## Return Value

YES if the element was activated or NO if it was not.

## Discussion

You can use this method to make complex controls more readily accessible to users. The accessibility system calls this method when a VoiceOver user double taps the selected element. Your implementation of this method should activate the element and perform whatever other tasks it deems appropriate. For example, you might use the method to activate a control that requires a complex gesture and would be difficult for VoiceOver users to perform, possibly because the gesture has a different meaning when VoiceOver is running.

After performing any tasks, return an appropriate Boolean value to indicate success or failure.

## See Also

### Performing an action

func accessibilityIncrement()

Tells the accessibility element to increment the value of its content.

func accessibilityDecrement()

Tells the accessibility element to decrement the value of its content.

func accessibilityScroll(UIAccessibilityScrollDirection) -> Bool

Scrolls screen content in an application-specific way and returns the success or failure of the action.

func accessibilityPerformEscape() -> Bool

Dismisses a modal view and returns the success or failure of the action.

func accessibilityPerformMagicTap() -> Bool

Performs a salient action.

