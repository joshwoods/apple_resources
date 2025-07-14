

- TVMLKit
- TVDocumentViewController
-  documentContext Deprecated

Instance Property

# documentContext

The current document context.

tvOS 13.0–18.0Deprecated

``` source
@MainActor
var documentContext: [String : Any] { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

Use this property to retrieve the current context, whether it’s new or updated.

## See Also

### Accessing the Document’s Components

var appController: TVApplicationController?

The document’s app controller that bridges UI, navigation stack, storage, and event handling from JavaScript.

Deprecated

