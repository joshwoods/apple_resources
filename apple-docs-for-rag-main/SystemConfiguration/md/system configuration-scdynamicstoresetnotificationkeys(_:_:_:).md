

- System Configuration
-  SCDynamicStoreSetNotificationKeys(\_:\_:\_:) 

Function

# SCDynamicStoreSetNotificationKeys(\_:\_:\_:)

Specifies a set of keys and key patterns that should be monitored for changes.

macOS 10.1+

``` source
func SCDynamicStoreSetNotificationKeys(
    _ store: SCDynamicStore,
    _ keys: CFArray?,
    _ patterns: CFArray?
) -> Bool
```

## Parameters 

`store`  

The dynamic store session being watched.

`keys`  

An array of keys to be monitored or `NULL` if no specific keys are to be monitored.

`patterns`  

An array of regex(3) pattern strings used to match keys to be monitored or `NULL` if no key patterns are to be monitored.

## Return Value

`TRUE` if the set of notification keys and patterns was successfully updated; otherwise, `FALSE`.

## See Also

### Monitoring Keys and Values

func SCDynamicStoreNotifyValue(SCDynamicStore?, CFString) -> Bool

Causes a notification to be delivered for the specified key in the dynamic store.

func SCDynamicStoreSetDispatchQueue(SCDynamicStore, dispatch_queue_t?) -> Bool

Initiates notifications for the notification keys, using the specified dispatch queue for the callback.

