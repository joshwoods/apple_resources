

- AVFoundation
- AVAssetReaderTrackOutput
-  init(track:outputSettings:) 

Initializer

# init(track:outputSettings:)

Creates an object that reads media data from an asset track.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init(
    track: AVAssetTrack,
    outputSettings: [String : Any]?
)
```

## Parameters 

`track`  

The track from which to read media samples.

`outputSettings`  

A dictionary of settings to use for sample output. Specify `nil` to receive samples in their storage format.

You use keys and values from Audio settings, Video settings, or CVPixelBuffer, depending on the media type and the output format you require.

## See Also

### Creating a Track Output

Video settings

Configure video processing settings using standard key and value constants.

