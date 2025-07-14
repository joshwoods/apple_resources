

- Core Media
- CMSampleTimingInfo
-  presentationTimeStamp 

Instance Property

# presentationTimeStamp

The time at which the sample will be presented.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var presentationTimeStamp: CMTime
```

## Discussion

If a single struct applies to each of the samples, they all have this duration.

## See Also

### Properties

var decodeTimeStamp: CMTime

The time at which the sample will be decoded.

var duration: CMTime

The duration of the sample.

