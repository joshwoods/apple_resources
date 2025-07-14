

- Accelerate
- BNNS
-  BNNS.NearestNeighbors 

Structure

# BNNS.NearestNeighbors

A structure that calculates k-nearest neighbors.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct NearestNeighbors
```

## Overview

The following code generates eight 2D data points and loads them into a k-nearest neighbors object with a single call to the append(samples:) function. The code then computes the four nearest neighbors, based on Euclidean distance, to the sample data point at index 7 of the samples data.

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
let samplesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: samples,
    shape: .matrixRowMajor(8, 2))

let maximumSampleCount = 8
let dimensionCount = 2
let nearestNeighborCount = 4

let knn = BNNS.NearestNeighbors(
    capacity: maximumSampleCount,
    dimensionCount: dimensionCount,
    neighborCount: nearestNeighborCount,
    dataType: .float)

knn.append(samples: samplesDescriptor)

let indices = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Int32.self,
    shape: .vector(nearestNeighborCount))
let distances = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Int32.self,
    shape: .vector(nearestNeighborCount))

knn.apply(index: 7,
     outputIndices: indices,
     outputDistances: distances)
```

On return, the `indices` array contains the values `[7, 2, 4, 6]` and the distances array contains the values `[0.0, 1.4142135, 2.236068, 3.0]`.

## Topics

### Creating a k-nearest neighbors object

init(capacity: Int, dimensionCount: Int, neighborCount: Int, dataType: BNNSDataType)

Returns a new k-nearest neighbors object.

### Appending data points to a k-nearest neighbors object

func append(samples: BNNSNDArrayDescriptor)

Adds new sample data to a k-nearest neighbors object.

### Calculating k-nearest neighbors

func apply(index: Int?, outputIndices: BNNSNDArrayDescriptor, outputDistances: BNNSNDArrayDescriptor)

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

## See Also

### K-nearest neighbors calculation

typealias BNNSNearestNeighbors

A k-nearest neighbors object.

func BNNSCreateNearestNeighbors(UInt32, UInt32, UInt32, BNNSDataType, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSNearestNeighbors?

Returns a new k-nearest neighbors object.

func BNNSNearestNeighborsLoad(BNNSNearestNeighbors?, UInt32, UnsafeRawPointer) -> Int32

Adds new sample data to a k-nearest neighbors object.

func BNNSNearestNeighborsGetInfo(BNNSNearestNeighbors?, Int32, UnsafeMutablePointer&lt;Int32>?, UnsafeMutableRawPointer?) -> Int32

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

func BNNSDestroyNearestNeighbors(BNNSNearestNeighbors?)

Destroys a k-nearest neighbors object.

