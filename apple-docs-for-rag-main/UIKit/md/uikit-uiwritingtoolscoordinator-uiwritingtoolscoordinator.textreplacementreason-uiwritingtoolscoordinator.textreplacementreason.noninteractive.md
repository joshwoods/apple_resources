

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.TextReplacementReason
-  UIWritingToolsCoordinator.TextReplacementReason.noninteractive 

Case

# UIWritingToolsCoordinator.TextReplacementReason.noninteractive

An option to replace the text in your view without animating the change.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case noninteractive
```

## Discussion

When Writing Tools requests a noninteractive change in your delegate’s `UIWritingToolsCoordinator/Delegate/writingToolsCoordinator(_:replaceRange:inContext:proposedText:reason:animationParameters:completion:)` method, update your view’s text storage without animating the change.

## See Also

### Getting the reasons

case interactive

An option to animate the replacement of text in your view.

