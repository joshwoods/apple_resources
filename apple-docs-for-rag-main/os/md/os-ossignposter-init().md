

- os
- OSSignposter
-  init() 

Initializer

# init()

Creates a signposter that uses the default subsystem.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init()
```

## See Also

### Creating a Signposter

init(subsystem: String, category: String)

Creates a signposter that uses the specified subsystem and category.

init(subsystem: String, category: OSLog.Category)

Creates a signposter that uses the specified subsystem and system-defined log category.

init(logger: Logger)

Creates a signposter that uses the subsystem and category of an existing logger.

init(logHandle: OSLog)

Creates a signposter that uses the subsystem and category of an existing log.

static var disabled: OSSignposter

A shared signposter that doesn’t emit signposts at runtime.

