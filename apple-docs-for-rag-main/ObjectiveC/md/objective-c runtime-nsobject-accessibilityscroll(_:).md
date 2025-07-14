

- Objective-C Runtime
- NSObject
-  accessibilityScroll(\_:) 

Instance Method

# accessibilityScroll(\_:)

Scrolls screen content in an application-specific way and returns the success or failure of the action.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityScroll(_ direction: UIAccessibilityScrollDirection) -> Bool
```

## Parameters 

`direction`  

A constant that specifies the direction of the scrolling action. See UIAccessibilityScrollDirection for descriptions of valid constants.

## Return Value

YES if the scrolling action succeeds; otherwise, NO. By default, this method returns NO.

## Discussion

Implement this method if a view in the view hierarchy supports a scroll by page action.

- If the scrolling action succeeds for the specified direction, return YES and post the pageScrolled notification.

- If the scrolling action fails, `accessibilityScroll:` is called on a parent view in the hierarchy.

## See Also

### Performing an action

func accessibilityActivate() -> Bool

Tells the element to activate itself and report the success or failure of the operation.

func accessibilityIncrement()

Tells the accessibility element to increment the value of its content.

func accessibilityDecrement()

Tells the accessibility element to decrement the value of its content.

func accessibilityPerformEscape() -> Bool

Dismisses a modal view and returns the success or failure of the action.

func accessibilityPerformMagicTap() -> Bool

Performs a salient action.

