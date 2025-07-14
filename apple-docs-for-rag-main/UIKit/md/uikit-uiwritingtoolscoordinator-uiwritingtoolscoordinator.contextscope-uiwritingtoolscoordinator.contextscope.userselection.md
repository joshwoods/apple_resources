

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.ContextScope
-  UIWritingToolsCoordinator.ContextScope.userSelection 

Case

# UIWritingToolsCoordinator.ContextScope.userSelection

An option to provide only the view’s currently selected text.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case userSelection
```

## Discussion

With this option, include the selected text in your context object, along with some additional text before and after the selection. When performing changes inline with your view’s content, Writing Tools applies animations only to the selected text.

## See Also

### Getting the scope

case fullDocument

An option to provide all of your view’s text.

case visibleArea

An option to provide only the text in the currently visible portion of your view.

