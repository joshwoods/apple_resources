

- Core Foundation
-  CFNotificationCenterAddObserver(\_:\_:\_:\_:\_:\_:) 

Function

# CFNotificationCenterAddObserver(\_:\_:\_:\_:\_:\_:)

Registers an observer to receive notifications.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNotificationCenterAddObserver(
    _ center: CFNotificationCenter!,
    _ observer: UnsafeRawPointer!,
    _ callBack: CFNotificationCallback!,
    _ name: CFString!,
    _ object: UnsafeRawPointer!,
    _ suspensionBehavior: CFNotificationSuspensionBehavior
)
```

## Parameters 

`center`  

The notification center to which to add the observer.

`observer`  

The observer. In macOS 10.3 and later, this parameter may be `NULL`.

`callBack`  

The callback function to call when `object` posts the notification named `name`.

`name`  

The name of the notification to observe. If `NULL`, `callback` is called for any notification posted by `object`.

If `center` is a Darwin notification center, this value must *not* be `NULL`.

`object`  

The object to observe. For distributed notifications, `object` must be a CFString object. If `NULL`, `callback` is called when a notification named `name` is posted by any object.

If `center` is a Darwin notification center, this value is ignored.

`suspensionBehavior`  

Flag indicating how notifications should be handled when the application is in the background. See CFNotificationSuspensionBehavior for the list of available values.

If `center` is a Darwin notification center, this value is ignored.

## Discussion

Notification delivery is registered for the main thread.

If you need to control which thread processes a notification, your callback function must be able to forward the notification to the proper thread. You can use a `CFMessagePort` object or a custom `CFRunLoopSource` object to send notifications to the correct thread’s run loop.

## See Also

### Related Documentation

class CFRunLoopSource

class CFMessagePort

### Adding and Removing Observers

func CFNotificationCenterRemoveEveryObserver(CFNotificationCenter!, UnsafeRawPointer!)

Stops an observer from receiving any notifications from any object.

func CFNotificationCenterRemoveObserver(CFNotificationCenter!, UnsafeRawPointer!, CFNotificationName!, UnsafeRawPointer!)

Stops an observer from receiving certain notifications.

