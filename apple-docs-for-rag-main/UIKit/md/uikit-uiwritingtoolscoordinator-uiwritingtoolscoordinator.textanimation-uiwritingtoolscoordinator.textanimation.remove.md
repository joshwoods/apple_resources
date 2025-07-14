

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.TextAnimation
-  UIWritingToolsCoordinator.TextAnimation.remove 

Case

# UIWritingToolsCoordinator.TextAnimation.remove

The animation that Writing Tools performs when removing text from your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case remove
```

## Discussion

This type of animation shows the removal of text from your view. When preparing for this animation, hide the text in the provided range if you haven’t already. If you support animating the reflow of your view’s text, you can also prepare any other animations you need. Writing Tools uses a preview object you provide to animate the removal of the text.

## See Also

### Getting the animation types

case anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

case insert

The animation that Writing Tools performs when inserting text into your view.

