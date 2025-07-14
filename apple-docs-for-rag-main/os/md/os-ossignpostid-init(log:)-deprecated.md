

- os
- OSSignpostID
-  init(log:) Deprecated

Initializer

# init(log:)

Creates a signpost ID for the specified log.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
init(log: OSLog)
```

Deprecated

Use makeSignpostID() instead.

## Parameters 

`log`  

The log that you’re writing signposted events to.

## See Also

### Creating a Signpost Identifier

init(UInt64)

Creates a signpost ID from an arbitrary 64-bit integer value.

init(log: OSLog, object: AnyObject)

Creates a signpost ID and associates it with the specified object.

Deprecated

