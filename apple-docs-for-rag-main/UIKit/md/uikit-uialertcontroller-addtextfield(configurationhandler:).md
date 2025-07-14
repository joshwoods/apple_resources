

- UIKit
- UIAlertController
-  addTextField(configurationHandler:) 

Instance Method

# addTextField(configurationHandler:)

Adds a text field to an alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addTextField(configurationHandler: ((UITextField) -> Void)? = nil)
```

## Parameters 

`configurationHandler`  

A block for configuring the text field prior to displaying the alert. This block has no return value and takes a single parameter corresponding to the text field object. Use that parameter to change the text field properties.

## Discussion

Calling this method adds an editable text field to the alert. You can call this method more than once to add additional text fields. The text fields are stacked in the resulting alert.

You can add a text field only if the preferredStyle property is set to UIAlertController.Style.alert.

## See Also

### Configuring text fields

var textFields: [UITextField]?

The array of text fields displayed by the alert.

