

- Foundation
- NSException
-  userInfo 

Instance Property

# userInfo

A dictionary containing application-specific data pertaining to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get }
```

## Discussion

`nil` if no application-specific data exists. As an example, if a method’s return value caused the exception to be raised, the return value might be available to the exception handler through this method.

## See Also

### Related Documentation

init(name: NSExceptionName, reason: String?, userInfo: [AnyHashable : Any]?)

Initializes and returns a newly allocated exception object.

### Querying an NSException Object

var name: NSExceptionName

A string used to uniquely identify the receiver.

var reason: String?

A string containing a “human-readable” reason for the receiver.

