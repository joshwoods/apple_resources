

- UIKit
- UIActivityViewController
-  completionHandler Deprecated

Instance Property

# completionHandler

The completion handler to execute after the activity view controller is dismissed.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var completionHandler: UIActivityViewController.CompletionHandler? { get set }
```

Deprecated

Use the completionWithItemsHandler property instead.

## Discussion

When the user-selected service finishes operating on the data, or when the user dismisses the view controller, the view controller executes this completion handler to let your app know the final result of the operation.

## See Also

### Deprecated

typealias CompletionHandler

A completion handler to execute after the activity view controller is dismissed.

Deprecated

