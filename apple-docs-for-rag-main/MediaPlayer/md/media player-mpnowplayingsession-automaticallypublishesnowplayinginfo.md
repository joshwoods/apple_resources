

- Media Player
- MPNowPlayingSession
-  automaticallyPublishesNowPlayingInfo 

Instance Property

# automaticallyPublishesNowPlayingInfo

A Boolean that indicates whether Now Playing info automatically publishes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
var automaticallyPublishesNowPlayingInfo: Bool { get set }
```

## Discussion

You can set Now Playing information keys for automatic publishing on nowPlayingInfo.

Important

If you set `automaticallyPublishesNowPlayingInfo` to `true`, don’t use nowPlayingInfoCenter.

## See Also

### Configuring Now Playing information

var nowPlayingInfoCenter: MPNowPlayingInfoCenter

The Now Playing information center associated with the session.

