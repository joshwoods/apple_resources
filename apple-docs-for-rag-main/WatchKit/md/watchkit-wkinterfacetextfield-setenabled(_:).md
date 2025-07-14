

- WatchKit
- WKInterfaceTextField
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Enables or disables the text field.

watchOS 6.0+

``` source
func setEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

A Boolean value indicating whether the text field is enabled or disabled.

## Discussion

The `enabled` value determines whether the text field responds to user interaction. For enabled text fields, tapping the text field starts the text entry process. On watchOS, the system displays the text input controller. On nearby iOS devices associated with the same iCloud account, the system displays the Apple Remote Keyboard. A disabled text field does not respond to taps.

## See Also

### Configuring the Control

func setSecureTextEntry(Bool)

Determines whether the text field hides the text entered by the user.

