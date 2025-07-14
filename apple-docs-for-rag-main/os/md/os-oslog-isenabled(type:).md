

- os
- OSLog
-  isEnabled(type:) 

Instance Method

# isEnabled(type:)

Returns a Boolean value that indicates whether the log can write messages with the specified log type.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func isEnabled(type: OSLogType) -> Bool
```

## Parameters 

`type`  

A log type constant, such as OS_LOG_TYPE_DEFAULT, OS_LOG_TYPE_INFO, OS_LOG_TYPE_DEBUG, OS_LOG_TYPE_ERROR, or OS_LOG_TYPE_FAULT, that specifies the level of logging to check.

## Return Value

true if logging at the specified level is in an enabled state; otherwise, false.

