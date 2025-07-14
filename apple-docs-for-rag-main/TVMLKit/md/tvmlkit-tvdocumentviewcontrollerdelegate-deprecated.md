

- TVMLKit
-  TVDocumentViewControllerDelegate Deprecated

Protocol

# TVDocumentViewControllerDelegate

Methods to manage updates, events, and errors from the document view controller.

tvOS 13.0–18.0Deprecated

``` source
protocol TVDocumentViewControllerDelegate : NSObjectProtocol
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Managing Document Updates

func documentViewControllerWillUpdate(TVDocumentViewController)

Tells the delegate that the document will be updated.

func documentViewControllerDidUpdate(TVDocumentViewController)

Tells the delegate that the document has been updated.

func documentViewController(TVDocumentViewController, didUpdateWithContext: [String : Any])

Tells the delegate that the document has been updated with a specified context.

### Responding to Errors

func documentViewController(TVDocumentViewController, didFailUpdateWithError: any Error)

Tells the delegate that the document failed to update.

### Handling Events

func documentViewController(TVDocumentViewController, handleEvent: TVDocumentViewController.Event, with: TVViewElement) -> Bool

Handles events natively from document view controllers.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Interactions with the Document

var delegate: (any TVDocumentViewControllerDelegate)?

The delegate for handling events in the document view controller.

Deprecated

