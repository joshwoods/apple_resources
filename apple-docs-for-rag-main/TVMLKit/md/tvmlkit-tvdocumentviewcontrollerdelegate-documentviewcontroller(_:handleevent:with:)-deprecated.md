

- TVMLKit
- TVDocumentViewControllerDelegate
-  documentViewController(\_:handleEvent:with:) Deprecated

Instance Method

# documentViewController(\_:handleEvent:with:)

Handles events natively from document view controllers.

tvOS 13.0–18.0Deprecated

``` source
optional func documentViewController(
    _ documentViewController: TVDocumentViewController,
    handleEvent event: TVDocumentViewController.Event,
    with element: TVViewElement
) -> Bool
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

By default, event handling can happen in either `TVMLKit` or `TVMLKit JS`. To defer event handling exclusively to `TVMLKit JS`, return `false` and don’t handle the event in this `TVMLKit` method. To assign event handling to `TVMLKit`, handle the event in this method and return `true`.

