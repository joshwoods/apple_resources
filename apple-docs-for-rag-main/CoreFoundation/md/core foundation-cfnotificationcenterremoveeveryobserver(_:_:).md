

- Core Foundation
-  CFNotificationCenterRemoveEveryObserver(\_:\_:) 

Function

# CFNotificationCenterRemoveEveryObserver(\_:\_:)

Stops an observer from receiving any notifications from any object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNotificationCenterRemoveEveryObserver(
    _ center: CFNotificationCenter!,
    _ observer: UnsafeRawPointer!
)
```

## Parameters 

`center`  

The notification center from which to remove observers.

`observer`  

The observer. This value must not be `NULL`.

## Discussion

If you no longer want an observer to receive any notifications, perhaps because the observer is being deallocated, you can call this function to unregister the observer from all the notifications for which it had previously registered.

## See Also

### Adding and Removing Observers

func CFNotificationCenterAddObserver(CFNotificationCenter!, UnsafeRawPointer!, CFNotificationCallback!, CFString!, UnsafeRawPointer!, CFNotificationSuspensionBehavior)

Registers an observer to receive notifications.

func CFNotificationCenterRemoveObserver(CFNotificationCenter!, UnsafeRawPointer!, CFNotificationName!, UnsafeRawPointer!)

Stops an observer from receiving certain notifications.

