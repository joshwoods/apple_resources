

- AVFoundation
- AVAssetDownloadContentConfiguration
-  mediaSelections 

Instance Property

# mediaSelections

The media selections of an asset that a task downloads.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 10.0+

``` source
var mediaSelections: [AVMediaSelection] { get set }
```

## Discussion

If your configuration doesn’t indicate a media selection, the system uses the asset’s automatic media selection.

## See Also

### Accessing Configuration Details

var variantQualifiers: [AVAssetVariantQualifier]

The variant qualifiers for this configuration.

class AVAssetVariantQualifier

An object that represents an HTTP Live Streaming asset variant.

