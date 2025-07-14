

- Core Services
- File System Events
- FSEventStreamCreateFlags
-  kFSEventStreamCreateFlagIgnoreSelf 

Global Variable

# kFSEventStreamCreateFlagIgnoreSelf

Mac Catalyst 13.1+macOS 10.6+

``` source
var kFSEventStreamCreateFlagIgnoreSelf: Int { get }
```

## Discussion

Don't send events that were triggered by the current process. This is useful for reducing the volume of events that are sent. It is only useful if your process might modify the file system hierarchy beneath the path(s) being monitored. Note: this has no effect on historical events, i.e., those delivered before the HistoryDone sentinel event.

