

- Foundation
- Data
-  resetBytes(in:) 

Instance Method

# resetBytes(in:)

Sets a region of the data buffer to `0`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func resetBytes(in range: Range)
```

## Parameters 

`range`  

The range in the data to set to `0`.

## Discussion

If `range` exceeds the bounds of the data, then the data is resized to fit.

## See Also

### Creating Empty Data

init()

Creates an empty data buffer.

init(capacity: Int)

Creates an empty data buffer of a specified size.

init(count: Int)

Creates a new data buffer with the specified count of zeroed bytes.

