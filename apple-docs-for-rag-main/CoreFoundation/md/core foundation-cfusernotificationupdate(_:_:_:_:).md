

- Core Foundation
-  CFUserNotificationUpdate(\_:\_:\_:\_:) 

Function

# CFUserNotificationUpdate(\_:\_:\_:\_:)

Updates a displayed user notification dialog with new user interface information.

macOS 10.0+

``` source
func CFUserNotificationUpdate(
    _ userNotification: CFUserNotification!,
    _ timeout: CFTimeInterval,
    _ flags: CFOptionFlags,
    _ dictionary: CFDictionary!
) -> Int32
```

## Parameters 

`userNotification`  

The user notification to update.

`timeout`  

The new timeout value for the dialog.

`flags`  

A set of flags describing the type of notification to display. See CFUserNotificationCreate(_:_:_:_:_:) for details.

`dictionary`  

A description of the elements to display in the notification dialog. The possible keys are listed in Dialog Description Keys.

## Return Value

`0` if the cancel was successful; a non-`0` value otherwise.

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

func CFUserNotificationReceiveResponse(CFUserNotification!, CFTimeInterval, UnsafeMutablePointer&lt;CFOptionFlags>!) -> Int32

Waits for the user to respond to a notification or for the notification to time out.

func CFUserNotificationSecureTextField(CFIndex) -> CFOptionFlags

Returns a flag used to set the secure state of a text field.

