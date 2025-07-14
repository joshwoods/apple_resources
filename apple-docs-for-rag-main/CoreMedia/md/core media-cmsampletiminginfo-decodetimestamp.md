

- Core Media
- CMSampleTimingInfo
-  decodeTimeStamp 

Instance Property

# decodeTimeStamp

The time at which the sample will be decoded.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var decodeTimeStamp: CMTime
```

## Discussion

If the samples are in presentation order, this must be set to `kCMTimeInvalid`.

## See Also

### Properties

var duration: CMTime

The duration of the sample.

var presentationTimeStamp: CMTime

The time at which the sample will be presented.

