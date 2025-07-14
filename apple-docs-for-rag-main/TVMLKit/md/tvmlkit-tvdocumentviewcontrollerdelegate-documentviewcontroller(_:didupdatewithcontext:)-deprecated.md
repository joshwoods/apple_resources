

- TVMLKit
- TVDocumentViewControllerDelegate
-  documentViewController(\_:didUpdateWithContext:) Deprecated

Instance Method

# documentViewController(\_:didUpdateWithContext:)

Tells the delegate that the document has been updated with a specified context.

tvOS 13.0–18.0Deprecated

``` source
optional func documentViewController(
    _ documentViewController: TVDocumentViewController,
    didUpdateWithContext context: [String : Any]
)
```

Deprecated

Please use SwiftUI or UIKit

## See Also

### Managing Document Updates

func documentViewControllerWillUpdate(TVDocumentViewController)

Tells the delegate that the document will be updated.

Deprecated

func documentViewControllerDidUpdate(TVDocumentViewController)

Tells the delegate that the document has been updated.

Deprecated

