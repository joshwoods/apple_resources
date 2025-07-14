

- Core Foundation
- CFUserNotification
-  Button Flags 

API Collection

# Button Flags

Flags that alter the display of buttons in a user notification dialog.

## Overview

You specify these flags when you create the user notification with CFUserNotificationCreate(_:_:_:_:_:).

## Topics

### Constants

var kCFUserNotificationNoDefaultButtonFlag: CFOptionFlags

Displays the dialog without the default, alternate, or other buttons.

var kCFUserNotificationUseRadioButtonsFlag: CFOptionFlags

Creates a group of radio buttons instead of checkboxes for the elements in the kCFUserNotificationCheckBoxTitlesKey array in the user notification’s description dictionary.

## See Also

### Constants

Alert Levels

Flags identifying the seriousness of a user notification.

Response Codes

Response codes identifying the button that was pressed to dismiss a notification dialog.

Alert Levels

Flags identifying the seriousness of a user notification.

Response Codes

Response codes identifying the button that was pressed to dismiss a notification dialog.

Dialog Description Keys

Keys used in a user notification’s description dictionary, which describes the contents of the notification dialog to display.

