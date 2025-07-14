

- Core Foundation
-  CFNotificationCenterRemoveObserver(\_:\_:\_:\_:) 

Function

# CFNotificationCenterRemoveObserver(\_:\_:\_:\_:)

Stops an observer from receiving certain notifications.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNotificationCenterRemoveObserver(
    _ center: CFNotificationCenter!,
    _ observer: UnsafeRawPointer!,
    _ name: CFNotificationName!,
    _ object: UnsafeRawPointer!
)
```

## Parameters 

`center`  

The notification center to modify.

`observer`  

The observer. This value must not be `NULL`.

`name`  

The name of the notification to stop observing. If `NULL`, `observer` stops receiving callbacks for all notifications posted by `object`.

`object`  

The object to stop observing. For distributed notifications, `object` must be a CFString object. If `NULL`, `observer` stops receiving callbacks for all objects posting notifications named `name`.

If `center` is a Darwin notification center, this value is ignored.

## Discussion

If both `name` and `object` are `NULL`, this function unregisters `observer` from all the notifications for which it had previously registered with `center`.

## See Also

### Adding and Removing Observers

func CFNotificationCenterAddObserver(CFNotificationCenter!, UnsafeRawPointer!, CFNotificationCallback!, CFString!, UnsafeRawPointer!, CFNotificationSuspensionBehavior)

Registers an observer to receive notifications.

func CFNotificationCenterRemoveEveryObserver(CFNotificationCenter!, UnsafeRawPointer!)

Stops an observer from receiving any notifications from any object.

