

- Core Foundation
-  CFNotificationCenterGetLocalCenter() 

Function

# CFNotificationCenterGetLocalCenter()

Returns the application’s local notification center.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNotificationCenterGetLocalCenter() -> CFNotificationCenter!
```

## Return Value

The application’s local notification center. An application has only one local notification center, so this function returns the same value each time it is called.

## See Also

### Accessing a Notification Center

func CFNotificationCenterGetDarwinNotifyCenter() -> CFNotificationCenter!

Returns the application’s Darwin notification center.

func CFNotificationCenterGetDistributedCenter() -> CFNotificationCenter!

Returns the application’s distributed notification center.

