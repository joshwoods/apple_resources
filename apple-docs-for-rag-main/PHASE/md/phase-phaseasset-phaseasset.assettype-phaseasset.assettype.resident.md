

- PHASE
- PHASEAsset
- PHASEAsset.AssetType
-  PHASEAsset.AssetType.resident 

Case

# PHASEAsset.AssetType.resident

A sound asset that plays after fully loading in memory.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case resident
```

## Discussion

If the sound asset is in memory, the framework prepares it for playback. If the asset is on disk, the framework loads it into memory, and prepares it for playback.

## See Also

### Types

case streamed

A sound asset that streams from disk into memory as it plays.

