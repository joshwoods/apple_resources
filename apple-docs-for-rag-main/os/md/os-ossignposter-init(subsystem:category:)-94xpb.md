

- os
- OSSignposter
-  init(subsystem:category:) 

Initializer

# init(subsystem:category:)

Creates a signposter that uses the specified subsystem and category.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    subsystem: String,
    category: String
)
```

## Parameters 

`subsystem`  

The string that identifies the subsystem that emits signposts. Typically, you use the same value as your app’s *bundle ID*. For more information, see CFBundleIdentifier.

`category`  

The string that the system uses to categorize emitted signposts.

## See Also

### Creating a Signposter

init()

Creates a signposter that uses the default subsystem.

init(subsystem: String, category: OSLog.Category)

Creates a signposter that uses the specified subsystem and system-defined log category.

init(logger: Logger)

Creates a signposter that uses the subsystem and category of an existing logger.

init(logHandle: OSLog)

Creates a signposter that uses the subsystem and category of an existing log.

static var disabled: OSSignposter

A shared signposter that doesn’t emit signposts at runtime.

