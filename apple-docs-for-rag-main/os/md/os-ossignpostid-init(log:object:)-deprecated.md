

- os
- OSSignpostID
-  init(log:object:) Deprecated

Initializer

# init(log:object:)

Creates a signpost ID and associates it with the specified object.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
init(
    log: OSLog,
    object: AnyObject
)
```

Deprecated

Use makeSignpostID(from:) instead.

## Parameters 

`log`  

The log that you’re writing signposted events to.

`object`  

The object to associate with this signpost ID.

## Discussion

Important

Don’t use this method if your signpost IDs cross process boundaries.

## See Also

### Creating a Signpost Identifier

init(UInt64)

Creates a signpost ID from an arbitrary 64-bit integer value.

init(log: OSLog)

Creates a signpost ID for the specified log.

Deprecated

