

- AVFoundation
- AVCompositionTrack
-  preferredTransform 

Instance Property

# preferredTransform

The track’s transform preference to apply to its visual content during presentation or processing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var preferredTransform: CGAffineTransform { get }
```

## Discussion

The value of this property is typically, but not always, CGAffineTransformIdentity.

## See Also

### Accessing Visual Characteristics

var naturalSize: CGSize

The natural dimensions of the media data that the track references.

