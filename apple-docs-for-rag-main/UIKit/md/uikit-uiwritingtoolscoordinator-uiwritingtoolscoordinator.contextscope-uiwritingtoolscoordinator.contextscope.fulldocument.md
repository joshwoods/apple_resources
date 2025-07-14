

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.ContextScope
-  UIWritingToolsCoordinator.ContextScope.fullDocument 

Case

# UIWritingToolsCoordinator.ContextScope.fullDocument

An option to provide all of your view’s text.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
case fullDocument
```

## Discussion

With this option, include all of the text your view manages. If your view has multiple text storage objects, create a separate context object for each one.

## See Also

### Getting the scope

case userSelection

An option to provide only the view’s currently selected text.

case visibleArea

An option to provide only the text in the currently visible portion of your view.

