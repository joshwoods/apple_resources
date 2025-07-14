

- Core Services
- Apple Events
- Apple Event Recording Event ID Constants
-  kAENotifyRecording 

Global Variable

# kAENotifyRecording

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAENotifyRecording: AEEventID { get }
```

## Discussion

Wildcard event class and event ID handled by a recording process in order to receive and record copies of recordable events sent to it by the Apple Event Manager. Scripting components install a handler for this event on behalf of a recording process when recording is turned on and remove the handler when recording is turned off.

