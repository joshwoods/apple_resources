

- Core Media
- CMSampleBuffer
-  totalSampleSize 

Instance Property

# totalSampleSize

The total size in bytes of sample data in the buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var totalSampleSize: Int { get }
```

## Discussion

If a sample buffer doesn’t contain same sizes, the value of this property is `0`.

## See Also

### Inspecting Size Information

var numSamples: Int

The number of media samples the buffer contains.

func sampleSizes() throws -> [Int]

Retrieves an array of sample sizes that represents each sample in a sample buffer.

func sampleSize(at: Int) -> Int

Returns the size of a sample in bytes.

