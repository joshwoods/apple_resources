

- Media Player
- MPNowPlayingInfoCenter
-  nowPlayingInfo 

Instance Property

# nowPlayingInfo

The current Now Playing information for the default Now Playing info center.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 5.0+visionOS 1.0+watchOS 5.0+

``` source
var nowPlayingInfo: [String : Any]? { get set }
```

## Discussion

To clear the now playing info center dictionary, set it to `nil`.

## See Also

### Working with the default Now Playing info center

class func `default`() -> MPNowPlayingInfoCenter

Returns the singleton Now Playing info center.

enum MPNowPlayingInfoMediaType

The type of media currently playing.

