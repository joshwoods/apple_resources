

- System Configuration
-  SCPreferencesScheduleWithRunLoop(\_:\_:\_:) 

Function

# SCPreferencesScheduleWithRunLoop(\_:\_:\_:)

Schedules commit and apply notifications for the specified preferences session using the specified run loop and mode.

macOS 10.4+

``` source
func SCPreferencesScheduleWithRunLoop(
    _ prefs: SCPreferences,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`runLoop`  

The run loop on which the notification should be scheduled. Do not pass `NULL`.

`runLoopMode`  

The run loop mode with which to schedule the notification. Do not pass `NULL`.

## Return Value

`TRUE` if the notifications are successfully scheduled; otherwise, `FALSE`.

## See Also

### Managing Notifications and Callbacks

func SCPreferencesSetCallback(SCPreferences, SCPreferencesCallBack?, UnsafeMutablePointer&lt;SCPreferencesContext>?) -> Bool

Assigns the specified callback to the specified preferences session.

func SCPreferencesUnscheduleFromRunLoop(SCPreferences, CFRunLoop, CFString) -> Bool

Unschedules commit and apply notifications for the specified preferences session from the specified run loop and mode.

func SCPreferencesSetDispatchQueue(SCPreferences, dispatch_queue_t?) -> Bool

Schedules commit and apply notifications for the specified preferences session using the specified dispatch queue.

