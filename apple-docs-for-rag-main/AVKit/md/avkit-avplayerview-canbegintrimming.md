

- AVKit
- AVPlayerView
-  canBeginTrimming 

Instance Property

# canBeginTrimming

A Boolean value that indicates whether the player view can begin trimming.

macOS 10.9+

``` source
@MainActor
var canBeginTrimming: Bool { get }
```

## Mentioned in 

Implementing Trimming in a macOS Player

## Discussion

Before calling beginTrimming(completionHandler:), check the value of this property to determine whether the player view and current media support trimming. This property value is false if the current controls style doesn’t support trimming, the media is content protected, or when playing HTTP Live Streaming media.

If you’re presenting a menu item to initiate trimming, a good place to perform this check is in the validateUserInterfaceItem(_:) method of NSDocument:

```
override func validateUserInterfaceItem(_ item: NSValidatedUserInterfaceItem) -> Bool {
    if item.action == #selector(beginTrimming) {
        return playerView.canBeginTrimming
    }
    return super.validateUserInterfaceItem(item)
}
```

## See Also

### Trimming Media

func beginTrimming(completionHandler: ((AVPlayerViewTrimResult) -> Void)?)

Puts the player view into trimming mode.

enum AVPlayerViewTrimResult

Constants that specify an action a user takes when trimming media in a player view.

