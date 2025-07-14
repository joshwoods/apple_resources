

- OSLog
- OSLogEntryFromProcess
-  process 

Instance Property

# process

The name of the process that made the entry.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var process: String { get }
```

**Required**

## See Also

### Identifying the Process Source

var activityIdentifier: os_activity_id_t

The activity identifier associated with the entry.

**Required**

var processIdentifier: pid_t

The process identifier that made the entry.

**Required**

var sender: String

The name of the binary image that made the entry.

**Required**

var threadIdentifier: UInt64

The identifier of the thread that made the entry.

**Required**

