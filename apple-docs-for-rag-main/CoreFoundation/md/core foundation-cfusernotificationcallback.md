

- Core Foundation
-  CFUserNotificationCallBack 

Type Alias

# CFUserNotificationCallBack

Callback invoked when an asynchronous user notification dialog is dismissed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFUserNotificationCallBack = (CFUserNotification?, CFOptionFlags) -> Void
```

## Parameters 

`userNotification`  

The user notification that was dismissed.

`responseFlags`  

On return, contains flags identifying how the notification was dismissed, the state of any checkboxes, and the selected item of the pop-up menu. See CFUserNotificationReceiveResponse(_:_:_:) for details.

