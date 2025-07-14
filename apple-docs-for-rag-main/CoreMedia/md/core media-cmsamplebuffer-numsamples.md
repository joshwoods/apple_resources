

- Core Media
- CMSampleBuffer
-  numSamples 

Instance Property

# numSamples

The number of media samples the buffer contains.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var numSamples: Int { get }
```

## Discussion

The value is `0` if an error occurs.

## See Also

### Inspecting Size Information

func sampleSizes() throws -> [Int]

Retrieves an array of sample sizes that represents each sample in a sample buffer.

func sampleSize(at: Int) -> Int

Returns the size of a sample in bytes.

var totalSampleSize: Int

The total size in bytes of sample data in the buffer.

