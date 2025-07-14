

- System Configuration
-  SCPreferencesSetDispatchQueue(\_:\_:) 

Function

# SCPreferencesSetDispatchQueue(\_:\_:)

Schedules commit and apply notifications for the specified preferences session using the specified dispatch queue.

macOS 10.6+

``` source
func SCPreferencesSetDispatchQueue(
    _ prefs: SCPreferences,
    _ queue: dispatch_queue_t?
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`queue`  

The dispatch queue on which to run the callback function.

## Return Value

`TRUE` if the notifications are successfully scheduled; otherwise, `FALSE`.

## See Also

### Managing Notifications and Callbacks

func SCPreferencesSetCallback(SCPreferences, SCPreferencesCallBack?, UnsafeMutablePointer&lt;SCPreferencesContext>?) -> Bool

Assigns the specified callback to the specified preferences session.

func SCPreferencesScheduleWithRunLoop(SCPreferences, CFRunLoop, CFString) -> Bool

Schedules commit and apply notifications for the specified preferences session using the specified run loop and mode.

func SCPreferencesUnscheduleFromRunLoop(SCPreferences, CFRunLoop, CFString) -> Bool

Unschedules commit and apply notifications for the specified preferences session from the specified run loop and mode.

