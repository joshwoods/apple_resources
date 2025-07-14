

- UIKit
- UIDocumentInteractionController
-  dismissPreview(animated:) 

Instance Method

# dismissPreview(animated:)

Dismisses the currently active document preview.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func dismissPreview(animated: Bool)
```

## Parameters 

`animated`  

Specify true to animate the dismissal of the document preview or false to dismiss it immediately.

## Discussion

Use this method to dismiss the document preview programmatically. The document interaction controller may also dismiss the document preview automatically in response to user actions.

## See Also

### Presenting and dismissing a document preview

func presentPreview(animated: Bool) -> Bool

Displays a full-screen preview of the target document.

