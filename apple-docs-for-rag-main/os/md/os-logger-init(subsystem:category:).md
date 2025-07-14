

- os
- Logger
-  init(subsystem:category:) 

Initializer

# init(subsystem:category:)

Creates a logger using the specified subsystem and category.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

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

### Creating a Logger

init()

Creates a logger that writes to the default subsystem.

init(OSLog)

Creates a logger that writes to the specified log.

class OSLog

A container of related log messages.

