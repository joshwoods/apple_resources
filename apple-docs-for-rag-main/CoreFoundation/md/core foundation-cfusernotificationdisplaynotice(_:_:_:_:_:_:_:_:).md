

- Core Foundation
-  CFUserNotificationDisplayNotice(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CFUserNotificationDisplayNotice(\_:\_:\_:\_:\_:\_:\_:\_:)

Displays a user notification dialog that does not need a user response.

macOS 10.0+

``` source
func CFUserNotificationDisplayNotice(
    _ timeout: CFTimeInterval,
    _ flags: CFOptionFlags,
    _ iconURL: CFURL!,
    _ soundURL: CFURL!,
    _ localizationURL: CFURL!,
    _ alertHeader: CFString!,
    _ alertMessage: CFString!,
    _ defaultButtonTitle: CFString!
) -> Int32
```

## Parameters 

`timeout`  

The amount of time to wait for the user to dismiss the notification dialog before the dialog dismisses itself. Pass `0` to have the dialog never time out.

`flags`  

A set of flags describing the type of notification dialog to display. The value is normally just the alert level from Alert Levels. If you don’t want a default button displayed, perform a bitwise-OR operation with the alert level and the constant kCFUserNotificationNoDefaultButtonFlag.

`iconURL`  

A file URL pointing to the icon to display in the dialog. If `NULL`, a default icon is used based on the notification’s alert level specified in `flags`.

`soundURL`  

Not used.

`localizationURL`  

A file URL pointing to a bundle that contains localized versions of the strings displayed in the dialog. Can be `NULL`.

`alertHeader`  

The title of the notification dialog. Cannot be `NULL`.

`alertMessage`  

The message string to display in the dialog. Can be `NULL`.

`defaultButtonTitle`  

The title of the default button. If `NULL`, the string `OK` is used.

## Return Value

`0` if the cancel was successful; a non-`0` value otherwise.

## Discussion

This function returns immediately. It does not wait for a user response after displaying the dialog.

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

