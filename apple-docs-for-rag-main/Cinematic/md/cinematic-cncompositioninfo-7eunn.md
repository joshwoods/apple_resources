

- Cinematic
-  CNCompositionInfo 

Class

# CNCompositionInfo

An object that enables you to add the appropriate number of tracks for a Cinematic asset.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
class CNCompositionInfo
```

## Topics

### Instance Methods

func insertTimeRange(CMTimeRange, of: CNAssetInfo, at: CMTime) throws

Inserts a timeRange of Cinematic source asset into the corresponding tracks of a composition.

## Relationships

### Inherits From

- CNAssetInfo

## See Also

### Reading and rendering

class CNAssetInfo

An object that provides Cinematic-specific information about an asset, including its tracks.

class CNRenderingSession

An object representing the context in which rendering occurs.

