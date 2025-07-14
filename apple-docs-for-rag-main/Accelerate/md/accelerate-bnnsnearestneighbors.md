

- Accelerate
-  BNNSNearestNeighbors 

Type Alias

# BNNSNearestNeighbors

A k-nearest neighbors object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias BNNSNearestNeighbors = UnsafeMutableRawPointer
```

## See Also

### K-nearest neighbors calculation

struct NearestNeighbors

A structure that calculates k-nearest neighbors.

func BNNSCreateNearestNeighbors(UInt32, UInt32, UInt32, BNNSDataType, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSNearestNeighbors?

Returns a new k-nearest neighbors object.

func BNNSNearestNeighborsLoad(BNNSNearestNeighbors?, UInt32, UnsafeRawPointer) -> Int32

Adds new sample data to a k-nearest neighbors object.

func BNNSNearestNeighborsGetInfo(BNNSNearestNeighbors?, Int32, UnsafeMutablePointer&lt;Int32>?, UnsafeMutableRawPointer?) -> Int32

Calculates the sorted indices and Euclidean distances of the k-nearest neighbors to a specified sample data point.

func BNNSDestroyNearestNeighbors(BNNSNearestNeighbors?)

Destroys a k-nearest neighbors object.

