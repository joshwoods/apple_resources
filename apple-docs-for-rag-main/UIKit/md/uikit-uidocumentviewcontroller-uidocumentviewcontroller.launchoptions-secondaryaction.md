

- UIKit
- UIDocumentViewController
- UIDocumentViewController.LaunchOptions
-  secondaryAction 

Instance Property

# secondaryAction

The launch scene’s secondary action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@NSCopying @MainActor
var secondaryAction: UIAction? { get set }
```

## Mentioned in 

Customizing a document-based app’s launch experience

## Discussion

Set this property to add a secondary action to the document launch scene. If you set this property, the system adds a button for the secondary action to the title view.

## See Also

### Adding actions

var primaryAction: UIAction?

The launch scene’s primary action.

