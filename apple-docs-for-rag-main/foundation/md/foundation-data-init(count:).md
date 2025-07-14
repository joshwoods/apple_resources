

- Foundation
- Data
-  init(count:) 

Initializer

# init(count:)

Creates a new data buffer with the specified count of zeroed bytes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(count: Int)
```

## Parameters 

`count`  

The number of bytes the data initially contains.

## See Also

### Creating Empty Data

init()

Creates an empty data buffer.

init(capacity: Int)

Creates an empty data buffer of a specified size.

func resetBytes(in: Range&lt;Data.Index>)

Sets a region of the data buffer to `0`.

