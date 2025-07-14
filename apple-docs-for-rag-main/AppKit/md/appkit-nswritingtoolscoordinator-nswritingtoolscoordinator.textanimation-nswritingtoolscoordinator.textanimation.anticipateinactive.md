

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.TextAnimation
-  NSWritingToolsCoordinator.TextAnimation.anticipateInactive 

Case

# NSWritingToolsCoordinator.TextAnimation.anticipateInactive

The animation effect that Writing Tools performs when the view is waiting for results, but the system isn’t actively evaluating the text.

macOS 15.2+

``` source
case anticipateInactive
```

## Discussion

When Writing Tools isn’t actively evaluating your text, it creates this animation. When preparing for this animation, display the text in the specified range with a foreground color of 50% grey.

## See Also

### Getting the animation types

case anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

case insert

The animation that Writing Tools performs when inserting text into your view.

case remove

The animation that Writing Tools performs when removing text from your view.

case translate

The animation effect that Writing Tools performs on text situated after the insertion point.

