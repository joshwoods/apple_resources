

- Objective-C Runtime
- NSObject
-  accessibilityDecrement() 

Instance Method

# accessibilityDecrement()

Tells the accessibility element to decrement the value of its content.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityDecrement()
```

## Discussion

If your element has the adjustable trait, you must implement this method. Use this method to decrement the value of the element. For example, a UISlider object uses this method to decrement its value by an appropriate amount.

## See Also

### Performing an action

func accessibilityActivate() -> Bool

Tells the element to activate itself and report the success or failure of the operation.

func accessibilityIncrement()

Tells the accessibility element to increment the value of its content.

func accessibilityScroll(UIAccessibilityScrollDirection) -> Bool

Scrolls screen content in an application-specific way and returns the success or failure of the action.

func accessibilityPerformEscape() -> Bool

Dismisses a modal view and returns the success or failure of the action.

func accessibilityPerformMagicTap() -> Bool

Performs a salient action.

