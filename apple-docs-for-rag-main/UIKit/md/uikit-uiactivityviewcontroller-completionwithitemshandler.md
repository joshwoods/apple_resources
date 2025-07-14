

- UIKit
- UIActivityViewController
-  completionWithItemsHandler 

Instance Property

# completionWithItemsHandler

The completion handler to execute after the activity view controller is dismissed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var completionWithItemsHandler: UIActivityViewController.CompletionWithItemsHandler? { get set }
```

## Discussion

When the user-selected service finishes operating on the data, or when the user dismisses the view controller, the view controller executes this completion handler to let your app know the final result of the operation.

## See Also

### Accessing the completion handler

typealias CompletionWithItemsHandler

A completion handler to execute after the activity view controller is dismissed.

