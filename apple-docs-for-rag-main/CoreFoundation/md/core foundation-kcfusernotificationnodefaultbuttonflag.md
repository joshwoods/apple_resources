

- Core Foundation
-  kCFUserNotificationNoDefaultButtonFlag 

Global Variable

# kCFUserNotificationNoDefaultButtonFlag

Displays the dialog without the default, alternate, or other buttons.

macOS 10.0+

``` source
var kCFUserNotificationNoDefaultButtonFlag: CFOptionFlags { get }
```

## Discussion

The dialog remains on screen until it times out or you cancel it with CFUserNotificationCancel(_:). If you provide a title for the default button in the user notification’s description dictionary, this flag is ignored and buttons show up normally.

## See Also

### Constants

var kCFUserNotificationUseRadioButtonsFlag: CFOptionFlags

Creates a group of radio buttons instead of checkboxes for the elements in the kCFUserNotificationCheckBoxTitlesKey array in the user notification’s description dictionary.

