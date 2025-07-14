

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.TextAnimation
-  NSWritingToolsCoordinator.TextAnimation.insert 

Case

# NSWritingToolsCoordinator.TextAnimation.insert

The animation that Writing Tools performs when inserting text into your view.

macOS 15.2+

``` source
case insert
```

## Discussion

This type of animation shows the insertion of text to your view. When preparing for this animation, hide the text in the provided range if you haven’t already. If you support animating the reflow of your view’s text, you can also prepare any other animations you need. Writing Tools uses a preview object you provide to animate the insertion of the text.

## See Also

### Getting the animation types

case anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

case remove

The animation that Writing Tools performs when removing text from your view.

case anticipateInactive

The animation effect that Writing Tools performs when the view is waiting for results, but the system isn’t actively evaluating the text.

case translate

The animation effect that Writing Tools performs on text situated after the insertion point.

