

- AVFoundation
- AVAssetExportSession
-  presetName 

Instance Property

# presetName

The name of the preset that the asset export session uses.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var presetName: String { get }
```

## Discussion

See Export Presets for values an asset export session supports.

This property is key-value observable.

## See Also

### Accessing Export Presets

func determineCompatibleFileTypes(completionHandler: ([AVFileType]) -> Void)

Determines the output file types an asset export session supports writing in its current configuration.

class func allExportPresets() -> [String]

Returns all available export preset names.

class func determineCompatibility(ofExportPreset: String, with: AVAsset, outputFileType: AVFileType?, completionHandler: (Bool) -> Void)

Determines an export preset’s compatibility to export the asset in a container of the output file type.

class func exportPresets(compatibleWith: AVAsset) -> [String]

Returns compatible export presets for the asset.

Deprecated

