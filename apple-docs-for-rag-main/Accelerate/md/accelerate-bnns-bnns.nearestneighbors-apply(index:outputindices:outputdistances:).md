

- Accelerate
- BNNS
- BNNS.NearestNeighbors
-  apply(index:outputIndices:outputDistances:) 

Instance Method

# apply(index:outputIndices:outputDistances:)

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func apply(
    index: Int?,
    outputIndices: BNNSNDArrayDescriptor,
    outputDistances: BNNSNDArrayDescriptor
)
```

## Parameters 

`index`  

The index of the sample data point of which the function computes the k-nearest neighbors.

`outputIndices`  

The sorted indices of the k-nearest neighbours to the sample data point.

`outputDistances`  

The sorted distances of the k-nearest neighbours to the sample data point.

