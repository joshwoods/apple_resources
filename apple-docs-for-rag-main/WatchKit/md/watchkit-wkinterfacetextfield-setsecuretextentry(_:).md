

- WatchKit
- WKInterfaceTextField
-  setSecureTextEntry(\_:) 

Instance Method

# setSecureTextEntry(\_:)

Determines whether the text field hides the text entered by the user.

watchOS 6.0+

``` source
func setSecureTextEntry(_ secureTextEntry: Bool)
```

## Discussion

Pass true to help keep passwords and other secure data private. When you enable secure text entry, the system displays a series of dots instead of the text entered by the user.

## See Also

### Configuring the Control

func setEnabled(Bool)

Enables or disables the text field.

