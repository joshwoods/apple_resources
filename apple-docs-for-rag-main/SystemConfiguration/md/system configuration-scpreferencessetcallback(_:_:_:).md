

- System Configuration
-  SCPreferencesSetCallback(\_:\_:\_:) 

Function

# SCPreferencesSetCallback(\_:\_:\_:)

Assigns the specified callback to the specified preferences session.

macOS 10.4+

``` source
func SCPreferencesSetCallback(
    _ prefs: SCPreferences,
    _ callout: SCPreferencesCallBack?,
    _ context: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`callout`  

The function to be called when the preferences have been changed or applied. If `NULL`, the current callback is removed.

`context`  

The context associated with the callback function. See SCPreferencesContext for more information about this structure.

## Return Value

`TRUE` if the callback was successfully associated with the preferences session; otherwise, `FALSE`.

## Discussion

This function is called when the changes to the preferences have been committed or applied.

## See Also

### Managing Notifications and Callbacks

func SCPreferencesScheduleWithRunLoop(SCPreferences, CFRunLoop, CFString) -> Bool

Schedules commit and apply notifications for the specified preferences session using the specified run loop and mode.

func SCPreferencesUnscheduleFromRunLoop(SCPreferences, CFRunLoop, CFString) -> Bool

Unschedules commit and apply notifications for the specified preferences session from the specified run loop and mode.

func SCPreferencesSetDispatchQueue(SCPreferences, dispatch_queue_t?) -> Bool

Schedules commit and apply notifications for the specified preferences session using the specified dispatch queue.

