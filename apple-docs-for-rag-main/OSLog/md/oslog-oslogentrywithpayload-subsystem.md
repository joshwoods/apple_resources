

- OSLog
- OSLogEntryWithPayload
-  subsystem 

Instance Property

# subsystem

The payload’s subsystem.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var subsystem: String { get }
```

**Required**

## Discussion

The category is derived from the `os_log_t` handle used.

## See Also

### Elements of a Payload

var category: String

The payload’s category.

**Required**

var components: [OSLogMessageComponent]

The payload’s components.

**Required**

var formatString: String

The payload’s format string.

**Required**

