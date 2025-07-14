

- AVFoundation
- AVMetadataObject
-  duration 

Instance Property

# duration

The duration of the media associated with this metadata object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
var duration: CMTime { get }
```

## Discussion

For metadata originating from a sample buffer (CMSampleBuffer), the duration reflects the duration of the sample buffer. If there is no valid duration value associated with the metadata, this property should contain invalid.

## See Also

### Getting the Media-Related Attributes

var time: CMTime

The media time value associated with the metadata object.

var bounds: CGRect

The bounding rectangle associated with the metadata.

