

- MediaExtension
- MEFileInfo
-  duration 

Instance Property

# duration

The duration of the media asset, if available.

macOS 14.0+

``` source
var duration: CMTime { get set }
```

## Discussion

This value is invalid if the duration isn’t available.

## See Also

### Inspecting file properties

var fragmentsStatus: MEFileInfo.FragmentsStatus

Indicates if the media asset contains fragments or is extendable by fragments.

enum FragmentsStatus

An enumeration that describes if a media asset contains or supports fragments.

