

- UIKit
- UIAlertController
-  textFields 

Instance Property

# textFields

The array of text fields displayed by the alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var textFields: [UITextField]? { get }
```

## Discussion

Use this property to access the text fields displayed by the alert. The text fields are in the order in which you added them to the alert controller. This order also corresponds to the order in which they are displayed in the alert.

## See Also

### Configuring text fields

func addTextField(configurationHandler: ((UITextField) -> Void)?)

Adds a text field to an alert.

