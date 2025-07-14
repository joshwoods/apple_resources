

- OSLog
- OSLogEntryWithPayload
-  components 

Instance Property

# components

The payload’s components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var components: [OSLogMessageComponent] { get }
```

**Required**

## Discussion

This property contains an array of OSLogMessageComponent objects from the composed message.

## See Also

### Elements of a Payload

var category: String

The payload’s category.

**Required**

var formatString: String

The payload’s format string.

**Required**

var subsystem: String

The payload’s subsystem.

**Required**

