

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.ContextScope
-  NSWritingToolsCoordinator.ContextScope.fullDocument 

Case

# NSWritingToolsCoordinator.ContextScope.fullDocument

An option to provide all of your view’s text.

macOS 15.2+

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

