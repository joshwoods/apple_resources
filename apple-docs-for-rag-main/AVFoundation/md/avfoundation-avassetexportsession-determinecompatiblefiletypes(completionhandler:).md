

- AVFoundation
- AVAssetExportSession
-  determineCompatibleFileTypes(completionHandler:) 

Instance Method

# determineCompatibleFileTypes(completionHandler:)

Determines the output file types an asset export session supports writing in its current configuration.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func determineCompatibleFileTypes(completionHandler handler: @escaping ([AVFileType]) -> Void)
```

``` source
var compatibleFileTypes: [AVFileType] { get async }
```

## Parameters 

`handler`  

A callback the system passes an array of AVFileType structures when it determines the compatible file types.

## See Also

### Accessing Export Presets

var presetName: String

The name of the preset that the asset export session uses.

class func allExportPresets() -> [String]

Returns all available export preset names.

class func determineCompatibility(ofExportPreset: String, with: AVAsset, outputFileType: AVFileType?, completionHandler: (Bool) -> Void)

Determines an export preset’s compatibility to export the asset in a container of the output file type.

class func exportPresets(compatibleWith: AVAsset) -> [String]

Returns compatible export presets for the asset.

Deprecated

