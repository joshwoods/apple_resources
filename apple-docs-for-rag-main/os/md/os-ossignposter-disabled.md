

- os
- OSSignposter
-  disabled 

Type Property

# disabled

A shared signposter that doesn’t emit signposts at runtime.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static var disabled: OSSignposter { get }
```

## Discussion

You can use the signposter this property returns to disable signposts in your production builds without having to refactor your code, as the following example demonstrates:

```
let signposter: OSSignposter
#if DEBUG
signposter = OSSignposter()
#else
signposter = OSSignposter.disabled
#endif
```

To determine if a signposter can emit signposts, use the isEnabled property.

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

init(logHandle: OSLog)

Creates a signposter that uses the subsystem and category of an existing log.

