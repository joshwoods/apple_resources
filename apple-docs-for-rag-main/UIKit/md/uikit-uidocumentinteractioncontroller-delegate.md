

- UIKit
- UIDocumentInteractionController
-  delegate 

Instance Property

# delegate

The delegate you want to receive document interaction notifications.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIDocumentInteractionControllerDelegate)? { get set }
```

## Discussion

You can implement a delegate object to track user interactions with menu items displayed by the document interaction controller. For more information, see UIDocumentInteractionControllerDelegate.

The default value of this property is `nil`.

## See Also

### Handling document-related interactions

protocol UIDocumentInteractionControllerDelegate

A set of methods you can implement to respond to messages from a document interaction controller.

