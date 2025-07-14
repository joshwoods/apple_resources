

- UIKit
- UITextCursorView
-  isBlinking 

Instance Property

# isBlinking

A Boolean value that determines whether the blink animation is running.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var isBlinking: Bool { get set }
```

**Required**

## Discussion

Set this property to true when you want the system to start animating the blink effect for the insertion point cursor. Set the property to false to stop the blink animation.

## See Also

### Determining the animation state

func resetBlinkAnimation()

Resets the blink animation to avoid glitches while someone is typing.

**Required**

