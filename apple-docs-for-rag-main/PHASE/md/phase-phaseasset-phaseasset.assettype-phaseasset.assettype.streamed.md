

- PHASE
- PHASEAsset
- PHASEAsset.AssetType
-  PHASEAsset.AssetType.streamed 

Case

# PHASEAsset.AssetType.streamed

A sound asset that streams from disk into memory as it plays.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case streamed
```

## Discussion

If the asset is on disk, the framework streams the asset’s data from disk into memory and prepares the asset during playback. If the asset is in memory, the framework streams from memory and prepares the asset during playback.

## See Also

### Types

case resident

A sound asset that plays after fully loading in memory.

