

- UIKit
- UITextCursorView
-  resetBlinkAnimation() 

Instance Method

# resetBlinkAnimation()

Resets the blink animation to avoid glitches while someone is typing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func resetBlinkAnimation()
```

**Required**

## Discussion

When the cursor is moving in your text view, call this method to prevent the insertion point from blinking.

## See Also

### Determining the animation state

var isBlinking: Bool

A Boolean value that determines whether the blink animation is running.

**Required**

