

- Core Foundation
-  CFUserNotificationCreate(\_:\_:\_:\_:\_:) 

Function

# CFUserNotificationCreate(\_:\_:\_:\_:\_:)

Creates a CFUserNotification object and displays its notification dialog on screen.

macOS 10.0+

``` source
func CFUserNotificationCreate(
    _ allocator: CFAllocator!,
    _ timeout: CFTimeInterval,
    _ flags: CFOptionFlags,
    _ error: UnsafeMutablePointer!,
    _ dictionary: CFDictionary!
) -> CFUserNotification!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`timeout`  

The time to wait before the notification dialog dismisses itself if the user does not respond. If `0`, the notification never times out.

`flags`  

A set of flags describing the type of notification to display. These flags specify an alert level for the notification (see Alert Levels), determine whether radio buttons or checkboxes are to be used (see Button Flags), specify which, if any, of these buttons are checked by default (see CFUserNotificationCheckBoxChecked(_:)), specify whether any of the text fields are to be secure text fields (see CFUserNotificationSecureTextField(_:)), and determine which element of a pop-up menu, if present, should be selected by default (see CFUserNotificationPopUpSelection(_:)). Combine these flags together by performing a bitwise-OR operation with all the individual flags.

`error`  

On return contains an integer error code. If `0`, the user notification was successfully created and displayed.

`dictionary`  

A description of the elements to display in the notification dialog. The possible keys are listed in Dialog Description Keys. The dictionary must contain a value for the key kCFUserNotificationAlertHeaderKey, but the other keys are optional.

## Return Value

The new CFUserNotification object. Ownership follows the The Create Rule.

## See Also

### CFUserNotification Miscellaneous Functions

func CFUserNotificationCancel(CFUserNotification!) -> Int32

Cancels a user notification dialog.

func CFUserNotificationCheckBoxChecked(CFIndex) -> CFOptionFlags

Returns a flag used to set or test a checkbox’s state.

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

