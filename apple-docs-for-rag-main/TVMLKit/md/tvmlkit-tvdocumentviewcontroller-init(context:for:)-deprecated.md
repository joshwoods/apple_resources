

- TVMLKit
- TVDocumentViewController
-  init(context:for:) Deprecated

Initializer

# init(context:for:)

Creates a new document view controller with a specific context and app controller.

tvOS 13.0–18.0Deprecated

``` source
@MainActor
convenience init(
    context: [String : Any],
    for appController: TVApplicationController
)
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The `context` parameter provides information to `TVMLKit JS` to determine which document to load.

