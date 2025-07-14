

- System Configuration
-  SCDynamicStoreSetDispatchQueue(\_:\_:) 

Function

# SCDynamicStoreSetDispatchQueue(\_:\_:)

Initiates notifications for the notification keys, using the specified dispatch queue for the callback.

macOS 10.6+

``` source
func SCDynamicStoreSetDispatchQueue(
    _ store: SCDynamicStore,
    _ queue: dispatch_queue_t?
) -> Bool
```

## Parameters 

`store`  

The dynamic store session.

`queue`  

The dispatch queue on which to run the callback function. Pass `NULL` to disable notifications and release the queue.

## Return Value

`TRUE` if notifications were successfully initiated; otherwise, `FALSE`.

## See Also

### Monitoring Keys and Values

func SCDynamicStoreNotifyValue(SCDynamicStore?, CFString) -> Bool

Causes a notification to be delivered for the specified key in the dynamic store.

func SCDynamicStoreSetNotificationKeys(SCDynamicStore, CFArray?, CFArray?) -> Bool

Specifies a set of keys and key patterns that should be monitored for changes.

