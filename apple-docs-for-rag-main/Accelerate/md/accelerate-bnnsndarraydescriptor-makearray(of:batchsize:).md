

- Accelerate
- BNNSNDArrayDescriptor
-  makeArray(of:batchSize:) 

Instance Method

# makeArray(of:batchSize:)

Returns a new array that contains a copy of the n-dimensional array descriptor’s data.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func makeArray(
    of scalarType: T.Type,
    batchSize: Int = 1
) -> [T]?
```

## Parameters 

`scalarType`  

The data type of the data.

`batchSize`  

The number of batches of data.

