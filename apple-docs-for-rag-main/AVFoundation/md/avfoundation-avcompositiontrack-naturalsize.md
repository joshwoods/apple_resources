

- AVFoundation
- AVCompositionTrack
-  naturalSize 

Instance Property

# naturalSize

The natural dimensions of the media data that the track references.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var naturalSize: CGSize { get }
```

## Discussion

For visual tracks, like video or subtitle tracks, this property value is the natural size of the media. For nonvisual tracks, like audio or chapter tracks, the value is zero.

## See Also

### Accessing Visual Characteristics

var preferredTransform: CGAffineTransform

The track’s transform preference to apply to its visual content during presentation or processing.

