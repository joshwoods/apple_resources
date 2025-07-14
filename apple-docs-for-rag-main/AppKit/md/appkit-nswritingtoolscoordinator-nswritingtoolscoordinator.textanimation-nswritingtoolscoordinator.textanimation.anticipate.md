

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.TextAnimation
-  NSWritingToolsCoordinator.TextAnimation.anticipate 

Case

# NSWritingToolsCoordinator.TextAnimation.anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

macOS 15.2+

``` source
case anticipate
```

## Discussion

This type of animation applies a visual effect to the text that Writing Tools is evaluating. When preparing for this animation, hide the text that Writing Tools is about to evaluate. In the same space where that text appears, Writing Tools displays a preview image that you provide and animates changes to that image.

## See Also

### Getting the animation types

case insert

The animation that Writing Tools performs when inserting text into your view.

case remove

The animation that Writing Tools performs when removing text from your view.

case anticipateInactive

The animation effect that Writing Tools performs when the view is waiting for results, but the system isn’t actively evaluating the text.

case translate

The animation effect that Writing Tools performs on text situated after the insertion point.

