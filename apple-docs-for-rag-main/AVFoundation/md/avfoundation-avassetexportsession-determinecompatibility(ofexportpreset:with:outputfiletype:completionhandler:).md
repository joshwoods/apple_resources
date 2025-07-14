

- AVFoundation
- AVAssetExportSession
-  determineCompatibility(ofExportPreset:with:outputFileType:completionHandler:) 

Type Method

# determineCompatibility(ofExportPreset:with:outputFileType:completionHandler:)

Determines an export preset’s compatibility to export the asset in a container of the output file type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func determineCompatibility(
    ofExportPreset presetName: String,
    with asset: AVAsset,
    outputFileType: AVFileType?,
    completionHandler handler: @escaping (Bool) -> Void
)
```

``` source
class func compatibility(
    ofExportPreset presetName: String,
    with asset: AVAsset,
    outputFileType: AVFileType?
) async -> Bool
```

## Parameters 

`presetName`  

The name of the preset whose compatibility you want to test. See Export Presets for preset values an asset export session supports.

`asset`  

The asset to export.

`outputFileType`  

The file type of the output container.

`handler`  

A callback the system passes a Boolean result when it determines the compatibility of the preset.

## See Also

### Accessing Export Presets

var presetName: String

The name of the preset that the asset export session uses.

func determineCompatibleFileTypes(completionHandler: ([AVFileType]) -> Void)

Determines the output file types an asset export session supports writing in its current configuration.

class func allExportPresets() -> [String]

Returns all available export preset names.

class func exportPresets(compatibleWith: AVAsset) -> [String]

Returns compatible export presets for the asset.

Deprecated

