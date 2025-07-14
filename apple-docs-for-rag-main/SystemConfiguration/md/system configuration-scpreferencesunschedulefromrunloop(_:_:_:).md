

- System Configuration
-  SCPreferencesUnscheduleFromRunLoop(\_:\_:\_:) 

Function

# SCPreferencesUnscheduleFromRunLoop(\_:\_:\_:)

Unschedules commit and apply notifications for the specified preferences session from the specified run loop and mode.

macOS 10.4+

``` source
func SCPreferencesUnscheduleFromRunLoop(
    _ prefs: SCPreferences,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`runLoop`  

The run loop from which the notification should be unscheduled. Do not pass `NULL`.

`runLoopMode`  

The run loop mode associated with the scheduled notification. Do not pass `NULL`.

## Return Value

`TRUE` if the notifications are successfully unscheduled; otherwise, `FALSE`.

## See Also

### Managing Notifications and Callbacks

func SCPreferencesSetCallback(SCPreferences, SCPreferencesCallBack?, UnsafeMutablePointer&lt;SCPreferencesContext>?) -> Bool

Assigns the specified callback to the specified preferences session.

func SCPreferencesScheduleWithRunLoop(SCPreferences, CFRunLoop, CFString) -> Bool

Schedules commit and apply notifications for the specified preferences session using the specified run loop and mode.

func SCPreferencesSetDispatchQueue(SCPreferences, dispatch_queue_t?) -> Bool

Schedules commit and apply notifications for the specified preferences session using the specified dispatch queue.

