

- os
- OSSignpostID
-  init(\_:) 

Initializer

# init(\_:)

Creates a signpost ID from an arbitrary 64-bit integer value.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
init(_ value: UInt64)
```

## Parameters 

`value`  

The value to use when generating the signpost ID.

## See Also

### Creating a Signpost Identifier

init(log: OSLog)

Creates a signpost ID for the specified log.

Deprecated

init(log: OSLog, object: AnyObject)

Creates a signpost ID and associates it with the specified object.

Deprecated

