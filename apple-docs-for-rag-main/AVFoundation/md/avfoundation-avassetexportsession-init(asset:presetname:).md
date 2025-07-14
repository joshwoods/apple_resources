

- AVFoundation
- AVAssetExportSession
-  init(asset:presetName:) 

Initializer

# init(asset:presetName:)

Creates an export session with a preset configuration.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init?(
    asset: AVAsset,
    presetName: String
)
```

## Parameters 

`asset`  

The asset to export.

`presetName`  

A string constant that specifies the preset template for the export. See Export Presets for available values.

## See Also

### Creating an Export Session

Export Presets

Configure an export session to output media in standard sizes and formats.

