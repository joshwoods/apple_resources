

- AVFoundation
- AVComposition
-  isExportable 

Instance Property

# isExportable

A Boolean value that indicates whether you can export this asset using an export session.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var isExportable: Bool { get }
```

## Discussion

This property value is true if you can export the composition using AVAssetExportSession.

## See Also

### Determining Suitability

var isPlayable: Bool

A Boolean value that indicates whether the asset has playable content.

var isReadable: Bool

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

var isComposable: Bool

A Boolean value that indicates whether you can use the asset as a segment of a composition track.

var isCompatibleWithAirPlayVideo: Bool

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

var isCompatibleWithSavedPhotosAlbum: Bool

A Boolean value that indicates whether you can write the composition to the Saved Photos album.

