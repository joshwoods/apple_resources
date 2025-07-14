

- Core Foundation
-  CFNotificationCenterGetDistributedCenter() 

Function

# CFNotificationCenterGetDistributedCenter()

Returns the application’s distributed notification center.

macOS

``` source
func CFNotificationCenterGetDistributedCenter() -> CFNotificationCenter!
```

## Return Value

The application’s distributed notification center. An application has only one distributed notification center, so this function returns the same value each time it is called.

## Discussion

A distributed notification center delivers notifications between applications. A notification object used with a distributed notification center must always be a CFString object and the notification dictionary must contain only property list values.

## See Also

### Accessing a Notification Center

func CFNotificationCenterGetDarwinNotifyCenter() -> CFNotificationCenter!

Returns the application’s Darwin notification center.

func CFNotificationCenterGetLocalCenter() -> CFNotificationCenter!

Returns the application’s local notification center.

