

- AVFoundation
- AVMetadataObject
-  time 

Instance Property

# time

The media time value associated with the metadata object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
var time: CMTime { get }
```

## Discussion

For captured media, this property represents the time when the metadata was captured. For metadata originating from a sample buffer (CMSampleBuffer), the time is the sample buffer’s presentation time. If there is no valid time value associated with the metadata, this property should contain invalid.

## See Also

### Getting the Media-Related Attributes

var duration: CMTime

The duration of the media associated with this metadata object.

var bounds: CGRect

The bounding rectangle associated with the metadata.

