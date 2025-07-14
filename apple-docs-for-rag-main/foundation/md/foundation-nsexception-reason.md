

- Foundation
- NSException
-  reason 

Instance Property

# reason

A string containing a “human-readable” reason for the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var reason: String? { get }
```

## See Also

### Related Documentation

init(name: NSExceptionName, reason: String?, userInfo: [AnyHashable : Any]?)

Initializes and returns a newly allocated exception object.

### Querying an NSException Object

var name: NSExceptionName

A string used to uniquely identify the receiver.

var userInfo: [AnyHashable : Any]?

A dictionary containing application-specific data pertaining to the receiver.

