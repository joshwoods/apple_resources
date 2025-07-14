

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.TextReplacementReason
-  NSWritingToolsCoordinator.TextReplacementReason.noninteractive 

Case

# NSWritingToolsCoordinator.TextReplacementReason.noninteractive

An option to replace the text in your view without animating the change.

macOS 15.2+

``` source
case noninteractive
```

## Discussion

When Writing Tools requests a noninteractive change in your delegate’s `NSWritingToolsCoordinator/writingToolsCoordinator(_:replaceRange:inContext:proposedText:reason:animationParameters:completion:)` method, update your view’s text storage without animating the change.

## See Also

### Getting the reasons

case interactive

An option to animate the replacement of text in your view.

