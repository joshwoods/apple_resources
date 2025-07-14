

- Accelerate
-  BNNSNearestNeighborsLoad(\_:\_:\_:) 

Function

# BNNSNearestNeighborsLoad(\_:\_:\_:)

Adds new sample data to a k-nearest neighbors object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func BNNSNearestNeighborsLoad(
    _ knn: BNNSNearestNeighbors?,
    _ n_new_samples: UInt32,
    _ data_ptr: UnsafeRawPointer
) -> Int32
```

## Parameters 

`knn`  

The k-nearest neighbors object.

`n_new_samples`  

The number of new samples.

`data_ptr`  

A pointer to the sample data. This must point to `n_new_samples * n_features` elements.

## Return Value

`0` when the load is successful; otherwise, a nonzero value.

## Discussion

The following code generates eight 2D data points and loads them into a k-nearest neighbors object with a single call to the BNNSNearestNeighborsLoad(_:_:_:) function. The code then computes the four nearest neighbors, based on Euclidean distance, to the sample data point at index 7 of the samples data.

```
let samples: [Float] = [
    1, 2,   // 0
    7, 2,   // 1
    3, 4,   // 2
    8, 4,   // 3
    3, 7,   // 4
    7, 7,   // 5
    2, 8,   // 6
    2, 5    // 7
]

let maximumSampleCount: UInt32 = 8
let dimensionCount: UInt32 = 2
let nearestNeighborCount: UInt32 = 4

let knn = BNNSCreateNearestNeighbors(
    maximumSampleCount,
    dimensionCount,
    nearestNeighborCount,
    BNNSDataType.float,
    nil)

defer {
    BNNSDestroyNearestNeighbors(knn)
}

BNNSNearestNeighborsLoad(
    knn,
    UInt32(samples.count) / dimensionCount,
    samples)

var indices = [Int32](repeating: 0,
                      count: Int(nearestNeighborCount))
var distances = [Float](repeating: 0,
                        count: Int(nearestNeighborCount))

let sampleDataPointIndex = 7
BNNSNearestNeighborsGetInfo(
    knn,
    Int32(sampleDataPointIndex),
    &indices,
    &distances)
```

On return, the `indices` array contains the values `[7, 2, 4, 6]` and the distances array contains the values `[0.0, 1.4142135, 2.236068, 3.0]`.

## See Also

### K-nearest neighbors calculation

struct NearestNeighbors

A structure that calculates k-nearest neighbors.

typealias BNNSNearestNeighbors

A k-nearest neighbors object.

func BNNSCreateNearestNeighbors(UInt32, UInt32, UInt32, BNNSDataType, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSNearestNeighbors?

Returns a new k-nearest neighbors object.

func BNNSNearestNeighborsGetInfo(BNNSNearestNeighbors?, Int32, UnsafeMutablePointer&lt;Int32>?, UnsafeMutableRawPointer?) -> Int32

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

func BNNSDestroyNearestNeighbors(BNNSNearestNeighbors?)

Destroys a k-nearest neighbors object.

