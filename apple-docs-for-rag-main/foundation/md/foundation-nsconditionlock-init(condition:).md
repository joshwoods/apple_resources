

- Foundation
- NSConditionLock
-  init(condition:) 

Initializer

# init(condition:)

Initializes a newly allocated `NSConditionLock` object and sets its condition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(condition: Int)
```

## Parameters 

`condition`  

The user-defined condition for the lock. The value of `condition` is user-defined; see the class description for more information.

## Return Value

An initialized condition lock object; may be different than the original receiver.

## See Also

### Related Documentation

Threading Programming Guide

