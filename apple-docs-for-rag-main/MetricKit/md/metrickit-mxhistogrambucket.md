

- MetricKit
-  MXHistogramBucket 

Class

# MXHistogramBucket

An object representing a bucket of data in a histogram.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
class MXHistogramBucket where UnitType : Unit
```

## Topics

### Reading the Data

var bucketStart: Measurement&lt;UnitType>

The value of the starting measurement for the bucket.

var bucketEnd: Measurement&lt;UnitType>

The value of the ending measurement for the bucket.

var bucketCount: Int

An integer representing the number of samples in the bucket.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Reading the buckets

var bucketEnumerator: NSEnumerator

An enumerator for the buckets containing the data in the histogram.

var totalBucketCount: Int

The total number of buckets in the histogram.

