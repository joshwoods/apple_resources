

- AVFoundation
- AVMutableMovie
-  isReadable 

Instance Property

# isReadable

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
var isReadable: Bool { get }
```

## Discussion

This property value is true if you can use AVAssetReader to extract the composition’s media data.

## See Also

### Determining Suitability

var isPlayable: Bool

A Boolean value that indicates whether the asset has playable content.

var isExportable: Bool

A Boolean value that indicates whether you can export this asset using an export session.

var isComposable: Bool

A Boolean value that indicates whether you can use the asset as a segment of a composition track.

var isCompatibleWithAirPlayVideo: Bool

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

var isCompatibleWithSavedPhotosAlbum: Bool

A Boolean value that indicates whether you can write the composition to the Saved Photos album.

