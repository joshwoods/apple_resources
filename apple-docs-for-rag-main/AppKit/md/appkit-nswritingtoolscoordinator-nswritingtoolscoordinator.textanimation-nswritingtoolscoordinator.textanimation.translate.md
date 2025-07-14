

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.TextAnimation
-  NSWritingToolsCoordinator.TextAnimation.translate 

Case

# NSWritingToolsCoordinator.TextAnimation.translate

The animation effect that Writing Tools performs on text situated after the insertion point.

macOS 15.2+

``` source
case translate
```

## Discussion

When Writing Tools inserts text at a given location, it creates an animation to make room for the new text. When preparing for this animation, hide the text between the insertion point and the end of your text storage. When finishing the animation, show the text again.

## See Also

### Getting the animation types

case anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

case insert

The animation that Writing Tools performs when inserting text into your view.

case remove

The animation that Writing Tools performs when removing text from your view.

case anticipateInactive

The animation effect that Writing Tools performs when the view is waiting for results, but the system isn’t actively evaluating the text.

