

- Cinematic
- CNCompositionInfo
-  insertTimeRange(\_:of:at:) 

Instance Method

# insertTimeRange(\_:of:at:)

Inserts a timeRange of Cinematic source asset into the corresponding tracks of a composition.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func insertTimeRange(
    _ timeRange: CMTimeRange,
    of cinematicAssetInfo: CNAssetInfo,
    at startTime: CMTime
) throws
```

## Parameters 

`timeRange`  

The time range where to insert the Cinematic source asset.

`cinematicAssetInfo`  

The asset to insert.

`startTime`  

The starting time where to insert the corresponding tracks of the composition.

