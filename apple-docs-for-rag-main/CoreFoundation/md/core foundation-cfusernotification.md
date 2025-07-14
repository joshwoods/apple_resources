

- Core Foundation
-  CFUserNotification 

Class

# CFUserNotification

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFUserNotification
```

## Overview

A `CFUserNotification` object presents a simple dialog on the screen and optionally receives feedback from the user. The contents of the dialog can include a header, a message, an icon, text fields, a pop-up button, radio buttons or checkboxes, and up to three ordinary buttons. Use `CFUserNotification` in processes that do not otherwise have user interfaces, but may need occasional interaction with the user.

You create a user notification with the CFUserNotificationCreate(_:_:_:_:_:) function. You pass in a dictionary whose keys describe the items to place into the dialog. (See Dialog Description Keys for the list of keys.) A set of flags passed to the function determines, among other things, whether secure text fields are used (such as for password fields), whether radio buttons or checkboxes are used, and which of these buttons are checked by default. You can also specify a timeout for the dialog, in which case the dialog cancels itself if the user does not respond in the allotted time period.

A user notification displays its dialog as soon as it is created. If any reply is required, it may be awaited in one of two ways: either synchronously, using CFUserNotificationReceiveResponse(_:_:_:), or asynchronously, using a run loop source created with CFUserNotificationCreateRunLoopSource(_:_:_:_:). CFUserNotificationReceiveResponse(_:_:_:) has a timeout parameter that determines how long it will block (zero meaning indefinitely) and it may be called as many times as necessary until a response arrives. If a user notification has not yet received a response, it may be updated with new information or it may be cancelled. User notifications may not be reused.

`CFUserNotification` provides two convenience functions, CFUserNotificationDisplayNotice(_:_:_:_:_:_:_:_:) and CFUserNotificationDisplayAlert(_:_:_:_:_:_:_:_:_:_:_:), to display very basic dialogs that either require no response from the user or require only a single button to be pressed, respectively.

## Topics

### CFUserNotification Miscellaneous Functions

func CFUserNotificationCancel(CFUserNotification!) -> Int32

Cancels a user notification dialog.

func CFUserNotificationCheckBoxChecked(CFIndex) -> CFOptionFlags

Returns a flag used to set or test a checkbox’s state.

func CFUserNotificationCreate(CFAllocator!, CFTimeInterval, CFOptionFlags, UnsafeMutablePointer&lt;Int32>!, CFDictionary!) -> CFUserNotification!

Creates a CFUserNotification object and displays its notification dialog on screen.

func CFUserNotificationCreateRunLoopSource(CFAllocator!, CFUserNotification!, CFUserNotificationCallBack!, CFIndex) -> CFRunLoopSource!

Creates a run loop source for a user notification.

func CFUserNotificationDisplayAlert(CFTimeInterval, CFOptionFlags, CFURL!, CFURL!, CFURL!, CFString!, CFString!, CFString!, CFString!, CFString!, UnsafeMutablePointer&lt;CFOptionFlags>!) -> Int32

Displays a user notification dialog and waits for a user response.

func CFUserNotificationDisplayNotice(CFTimeInterval, CFOptionFlags, CFURL!, CFURL!, CFURL!, CFString!, CFString!, CFString!) -> Int32

Displays a user notification dialog that does not need a user response.

func CFUserNotificationGetResponseDictionary(CFUserNotification!) -> CFDictionary!

Returns the dictionary containing all the text field values from a dismissed notification dialog.

func CFUserNotificationGetResponseValue(CFUserNotification!, CFString!, CFIndex) -> CFString!

Extracts the values of the text fields from a dismissed notification dialog.

func CFUserNotificationGetTypeID() -> CFTypeID

Returns the type identifier for the `CFUserNotification` opaque type.

func CFUserNotificationPopUpSelection(CFIndex) -> CFOptionFlags

Returns a flag used to set the selected element of a pop-up menu.

func CFUserNotificationReceiveResponse(CFUserNotification!, CFTimeInterval, UnsafeMutablePointer&lt;CFOptionFlags>!) -> Int32

Waits for the user to respond to a notification or for the notification to time out.

func CFUserNotificationSecureTextField(CFIndex) -> CFOptionFlags

Returns a flag used to set the secure state of a text field.

func CFUserNotificationUpdate(CFUserNotification!, CFTimeInterval, CFOptionFlags, CFDictionary!) -> Int32

Updates a displayed user notification dialog with new user interface information.

### Callbacks

typealias CFUserNotificationCallBack

Callback invoked when an asynchronous user notification dialog is dismissed.

### Constants

Alert Levels

Flags identifying the seriousness of a user notification.

Response Codes

Response codes identifying the button that was pressed to dismiss a notification dialog.

Button Flags

Flags that alter the display of buttons in a user notification dialog.

Alert Levels

Flags identifying the seriousness of a user notification.

Response Codes

Response codes identifying the button that was pressed to dismiss a notification dialog.

Button Flags

Flags that alter the display of buttons in a user notification dialog.

Dialog Description Keys

Keys used in a user notification’s description dictionary, which describes the contents of the notification dialog to display.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

