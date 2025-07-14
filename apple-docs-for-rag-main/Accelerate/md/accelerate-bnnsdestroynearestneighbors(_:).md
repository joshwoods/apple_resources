

- Accelerate
-  BNNSDestroyNearestNeighbors(\_:) 

Function

# BNNSDestroyNearestNeighbors(\_:)

Destroys a k-nearest neighbors object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func BNNSDestroyNearestNeighbors(_ knn: BNNSNearestNeighbors?)
```

## Parameters 

`knn`  

The k-nearest neighbors object.

## See Also

### K-nearest neighbors calculation

struct NearestNeighbors

A structure that calculates k-nearest neighbors.

typealias BNNSNearestNeighbors

A k-nearest neighbors object.

func BNNSCreateNearestNeighbors(UInt32, UInt32, UInt32, BNNSDataType, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSNearestNeighbors?

Returns a new k-nearest neighbors object.

func BNNSNearestNeighborsLoad(BNNSNearestNeighbors?, UInt32, UnsafeRawPointer) -> Int32

Adds new sample data to a k-nearest neighbors object.

func BNNSNearestNeighborsGetInfo(BNNSNearestNeighbors?, Int32, UnsafeMutablePointer&lt;Int32>?, UnsafeMutableRawPointer?) -> Int32

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

