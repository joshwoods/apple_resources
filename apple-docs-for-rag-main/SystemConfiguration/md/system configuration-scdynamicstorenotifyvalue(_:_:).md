

- System Configuration
-  SCDynamicStoreNotifyValue(\_:\_:) 

Function

# SCDynamicStoreNotifyValue(\_:\_:)

Causes a notification to be delivered for the specified key in the dynamic store.

macOS 10.1+

``` source
func SCDynamicStoreNotifyValue(
    _ store: SCDynamicStore?,
    _ key: CFString
) -> Bool
```

## Parameters 

`store`  

The dynamic store session.

`key`  

The key that should be flagged as changed. All dynamic store sessions that are monitoring this key will receive a notification. Note that the key’s value is not updated.

## Return Value

`TRUE` if the notification was processed; `FALSE` if an error occurred.

## See Also

### Monitoring Keys and Values

func SCDynamicStoreSetNotificationKeys(SCDynamicStore, CFArray?, CFArray?) -> Bool

Specifies a set of keys and key patterns that should be monitored for changes.

func SCDynamicStoreSetDispatchQueue(SCDynamicStore, dispatch_queue_t?) -> Bool

Initiates notifications for the notification keys, using the specified dispatch queue for the callback.

