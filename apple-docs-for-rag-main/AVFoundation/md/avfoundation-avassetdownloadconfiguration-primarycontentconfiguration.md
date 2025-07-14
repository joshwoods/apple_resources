

- AVFoundation
- AVAssetDownloadConfiguration
-  primaryContentConfiguration 

Instance Property

# primaryContentConfiguration

The configuration for the primary content that the task downloads.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 10.0+

``` source
var primaryContentConfiguration: AVAssetDownloadContentConfiguration { get }
```

## See Also

### Accessing Configuration Details

var artworkData: Data?

A data value that represents the asset’s artwork.

var auxiliaryContentConfigurations: [AVAssetDownloadContentConfiguration]

The configuration for the auxiliary content that the task downloads.

class AVAssetDownloadContentConfiguration

A configuration object that contains variant qualifiers and media options.

var optimizesAuxiliaryContentConfigurations: Bool

A Boolean value that indicates whether the task optimizes auxiliary content selection.

