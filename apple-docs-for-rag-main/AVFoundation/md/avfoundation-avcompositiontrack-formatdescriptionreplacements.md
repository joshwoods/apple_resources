

- AVFoundation
- AVCompositionTrack
-  formatDescriptionReplacements 

Instance Property

# formatDescriptionReplacements

The replacement format descriptions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var formatDescriptionReplacements: [AVCompositionTrackFormatDescriptionReplacement] { get }
```

## Discussion

The property’s values specify an original and a replacement format description, as set in a previous call to replaceFormatDescription(_:with:).

## See Also

### Managing Format Descriptions

var formatDescriptions: [Any]

The format descriptions of the media samples that a track references.

class AVCompositionTrackFormatDescriptionReplacement

An object that represents a format description and its replacement.

