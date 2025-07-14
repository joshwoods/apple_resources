

- AVFoundation
- AVAssetDownloadConfiguration
-  init(asset:title:) 

Initializer

# init(asset:title:)

Creates a download configuration for a media asset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 10.0+

``` source
convenience init(
    asset: AVURLAsset,
    title: String
)
```

## Parameters 

`asset`  

The asset the task downloads.

`title`  

A human-readable title for this asset. The system displays this value in the usage pane of the Settings app; choose a title suitable for display in the user’s preferred language.

