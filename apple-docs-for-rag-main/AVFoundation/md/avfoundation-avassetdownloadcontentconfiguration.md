

- AVFoundation
-  AVAssetDownloadContentConfiguration 

Class

# AVAssetDownloadContentConfiguration

A configuration object that contains variant qualifiers and media options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 10.0+

``` source
class AVAssetDownloadContentConfiguration
```

## Topics

### Accessing Configuration Details

var variantQualifiers: [AVAssetVariantQualifier]

The variant qualifiers for this configuration.

class AVAssetVariantQualifier

An object that represents an HTTP Live Streaming asset variant.

var mediaSelections: [AVMediaSelection]

The media selections of an asset that a task downloads.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Accessing Configuration Details

var artworkData: Data?

A data value that represents the asset’s artwork.

var primaryContentConfiguration: AVAssetDownloadContentConfiguration

The configuration for the primary content that the task downloads.

var auxiliaryContentConfigurations: [AVAssetDownloadContentConfiguration]

The configuration for the auxiliary content that the task downloads.

var optimizesAuxiliaryContentConfigurations: Bool

A Boolean value that indicates whether the task optimizes auxiliary content selection.

