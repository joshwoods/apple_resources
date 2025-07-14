

- AVFoundation
- AVAssetDownloadConfiguration
-  optimizesAuxiliaryContentConfigurations 

Instance Property

# optimizesAuxiliaryContentConfigurations

A Boolean value that indicates whether the task optimizes auxiliary content selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 10.0+

``` source
var optimizesAuxiliaryContentConfigurations: Bool { get set }
```

## Discussion

By default, a download task optimizes its selection of auxiliary content based on its primary download content. For example, if the primary content configuration represents stereo renditions, and auxiliary content configuration represents multichannel audio renditions, the task choses the auxiliary multichannel variant to avoid downloading duplicate video renditions.

## See Also

### Accessing Configuration Details

var artworkData: Data?

A data value that represents the asset’s artwork.

var primaryContentConfiguration: AVAssetDownloadContentConfiguration

The configuration for the primary content that the task downloads.

var auxiliaryContentConfigurations: [AVAssetDownloadContentConfiguration]

The configuration for the auxiliary content that the task downloads.

class AVAssetDownloadContentConfiguration

A configuration object that contains variant qualifiers and media options.

