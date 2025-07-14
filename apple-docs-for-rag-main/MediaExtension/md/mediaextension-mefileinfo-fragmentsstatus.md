

- MediaExtension
- MEFileInfo
-  fragmentsStatus 

Instance Property

# fragmentsStatus

Indicates if the media asset contains fragments or is extendable by fragments.

macOS 14.0+

``` source
var fragmentsStatus: MEFileInfo.FragmentsStatus { get set }
```

## Discussion

The default value is MEFileInfo.FragmentsStatus.couldNotContainFragments.

## See Also

### Inspecting file properties

var duration: CMTime

The duration of the media asset, if available.

enum FragmentsStatus

An enumeration that describes if a media asset contains or supports fragments.

