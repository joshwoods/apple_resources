

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.TextAnimation
-  UIWritingToolsCoordinator.TextAnimation.anticipate 

Case

# UIWritingToolsCoordinator.TextAnimation.anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

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

