

- Accelerate
- BNNS
- BNNS.NearestNeighbors
-  init(capacity:dimensionCount:neighborCount:dataType:) 

Initializer

# init(capacity:dimensionCount:neighborCount:dataType:)

Returns a new k-nearest neighbors object.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    capacity: Int,
    dimensionCount: Int,
    neighborCount: Int,
    dataType: BNNSDataType
)
```

## Parameters 

`capacity`  

The maximum number of data points.

`dimensionCount`  

The number of features or dimensions of each data point.

`neighborCount`  

The number of nearest neighbors that a subsequent call to apply(index:outputIndices:outputDistances:) calculates.

`dataType`  

The data type of the data points. This must be either `BNNSDataTypeFloat32` or `BNNSDataTypeFloat16`.

