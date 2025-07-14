

- UIKit
- UIDocumentViewController
- UIDocumentViewController.LaunchOptions
-  primaryAction 

Instance Property

# primaryAction

The launch scene’s primary action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@NSCopying @MainActor
var primaryAction: UIAction? { get set }
```

## Mentioned in 

Customizing a document-based app’s launch experience

## Discussion

Set this property to customize the primary action’s button in the document launch scene. If you don’t set this property, the system adds a default Create Document button to the title view.

## See Also

### Adding actions

var secondaryAction: UIAction?

The launch scene’s secondary action.

