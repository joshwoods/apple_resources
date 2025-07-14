

- UIKit
- UIAlertController
-  title 

Instance Property

# title

The title of the alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var title: String? { get set }
```

## Discussion

The title string is displayed prominently in the alert or action sheet. You should use this string to get the user’s attention and communicate the reason for displaying the alert.

## See Also

### Configuring the alert

var message: String?

Descriptive text that provides more details about the reason for the alert.

var preferredStyle: UIAlertController.Style

The style of the alert controller.

