

- os
- OSSignposter
-  init(logHandle:) 

Initializer

# init(logHandle:)

Creates a signposter that uses the subsystem and category of an existing log.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(logHandle: OSLog)
```

## Parameters 

`logHandle`  

The log that provides a subsystem and category for the signposter to use. For more information, see OSLog.

## See Also

### Creating a Signposter

init()

Creates a signposter that uses the default subsystem.

init(subsystem: String, category: String)

Creates a signposter that uses the specified subsystem and category.

init(subsystem: String, category: OSLog.Category)

Creates a signposter that uses the specified subsystem and system-defined log category.

init(logger: Logger)

Creates a signposter that uses the subsystem and category of an existing logger.

static var disabled: OSSignposter

A shared signposter that doesn’t emit signposts at runtime.

