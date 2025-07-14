

- Core Services
- File System Events
- FSEventStreamEventFlags
-  kFSEventStreamEventFlagEventIdsWrapped 

Global Variable

# kFSEventStreamEventFlagEventIdsWrapped

Mac Catalyst 13.0+macOS 10.5+

``` source
var kFSEventStreamEventFlagEventIdsWrapped: Int { get }
```

## Discussion

If kFSEventStreamEventFlagEventIdsWrapped is set, it means the 64-bit event ID counter wrapped around. As a result, previously-issued event ID's are no longer valid arguments for the sinceWhen parameter of the FSEventStreamCreate...() functions.

