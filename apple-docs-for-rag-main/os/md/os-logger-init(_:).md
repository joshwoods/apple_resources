

- os
- Logger
-  init(\_:) 

Initializer

# init(\_:)

Creates a logger that writes to the specified log.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init(_ logObj: OSLog)
```

## Parameters 

`logObj`  

The log to write messages to.

## See Also

### Creating a Logger

init()

Creates a logger that writes to the default subsystem.

init(subsystem: String, category: String)

Creates a logger using the specified subsystem and category.

class OSLog

A container of related log messages.

