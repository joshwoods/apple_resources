

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.TextReplacementReason
-  NSWritingToolsCoordinator.TextReplacementReason.interactive 

Case

# NSWritingToolsCoordinator.TextReplacementReason.interactive

An option to animate the replacement of text in your view.

macOS 15.2+

``` source
case interactive
```

## Discussion

When Writing Tools requests an interactive change in your delegate’s `NSWritingToolsCoordinator/writingToolsCoordinator(_:replaceRange:inContext:proposedText:reason:animationParameters:completion:)` method, it passes a valid set of animation parameters to that method. Update your view’s text storage and use the provided NSWritingToolsCoordinator.AnimationParameters type to create any view-specific animations you need to support the animated replacement of the text.

## See Also

### Getting the reasons

case noninteractive

An option to replace the text in your view without animating the change.

