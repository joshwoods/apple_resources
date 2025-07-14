

- UIKit
- UIAlertController
-  message 

Instance Property

# message

Descriptive text that provides more details about the reason for the alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var message: String? { get set }
```

## Discussion

The message string is displayed below the title string and is less prominent. Use this string to provide additional context about the reason for the alert or about the actions that the user might take.

## See Also

### Configuring the alert

var title: String?

The title of the alert.

var preferredStyle: UIAlertController.Style

The style of the alert controller.

