

- Accelerate
- BNNSNDArrayDescriptor
-  allocate(randomNormalUsing:mean:standardDeviation:shape:batchSize:) 

Type Method

# allocate(randomNormalUsing:mean:standardDeviation:shape:batchSize:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func allocate(
    randomNormalUsing: BNNS.RandomGenerator,
    mean: Scalar,
    standardDeviation: Scalar,
    shape: BNNS.Shape,
    batchSize: Int = 1
) -> BNNSNDArrayDescriptor? where Scalar : BNNSScalar, Scalar : BinaryFloatingPoint
```

