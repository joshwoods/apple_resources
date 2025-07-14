

- Objective-C Runtime
- NSObject
-  accessibilityPerformMagicTap() 

Instance Method

# accessibilityPerformMagicTap()

Performs a salient action.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityPerformMagicTap() -> Bool
```

## Return Value

YES if the magic tap action succeeds; otherwise, NO. By default, this method returns NO.

## Discussion

The exact action performed by this method depends your app, typically toggling the most important state of the app. For example, in the Phone app it answers and ends phone calls, in the Music app it plays and pauses playback, in the Clock app it starts and stops a timer, and in the Camera app it takes a picture.

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

func accessibilityPerformEscape() -> Bool

Dismisses a modal view and returns the success or failure of the action.

