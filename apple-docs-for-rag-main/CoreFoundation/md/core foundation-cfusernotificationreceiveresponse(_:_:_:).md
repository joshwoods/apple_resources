

- Core Foundation
-  CFUserNotificationReceiveResponse(\_:\_:\_:) 

Function

# CFUserNotificationReceiveResponse(\_:\_:\_:)

Waits for the user to respond to a notification or for the notification to time out.

macOS 10.0+

``` source
func CFUserNotificationReceiveResponse(
    _ userNotification: CFUserNotification!,
    _ timeout: CFTimeInterval,
    _ responseFlags: UnsafeMutablePointer!
) -> Int32
```

## Parameters 

`userNotification`  

The user notification to use.

`timeout`  

The amount of time to wait for the user to respond to `userNotification` or for the notification to time out. If neither happens before `timeout` passes, this function returns a non-`0` value. If `timeout` is `0`, the function blocks until the user notification is dismissed.

`responseFlags`  

On return, contains flags identifying how the notification was dismissed, the state of any checkboxes, and the selected element of the pop-up menu. Bits 0-1 of the value hold an identifier for the button pressed by the user (see Response Codes). Extract the identifier by performing a bitwise-AND operation with `0x3`. Bits 8-15 of `responseFlags` hold the state of up to 8 checkboxes or radio buttons, if present. Extract the flags by performing bitwise-AND operations with the return value of CFUserNotificationCheckBoxChecked(_:). Bits 24-31 hold the index number of the element selected in a pop-up menu, if present. Extract the index by performing a 24-bit right shift: `responseFlags >> 24`.

## Return Value

`0` if the call successfully received a response; a non-`0` value otherwise.

## Discussion

Use this function to poll a user notification for a user response. You can call it any number of times on the same user notification.

To avoid polling and blocking your thread’s execution, you can create a run loop source for the user notification with CFUserNotificationCreateRunLoopSource(_:_:_:_:). You will then receive a callback when the dialog is dismissed.

## See Also

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

func CFUserNotificationSecureTextField(CFIndex) -> CFOptionFlags

Returns a flag used to set the secure state of a text field.

func CFUserNotificationUpdate(CFUserNotification!, CFTimeInterval, CFOptionFlags, CFDictionary!) -> Int32

Updates a displayed user notification dialog with new user interface information.

