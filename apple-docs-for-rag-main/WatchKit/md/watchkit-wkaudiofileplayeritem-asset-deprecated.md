

- WatchKit
- WKAudioFilePlayerItem
-  asset Deprecated

Instance Property

# asset

The audio file asset being managed.

watchOS 2.0–6.0Deprecated

``` source
var asset: WKAudioFileAsset { get }
```

## Discussion

This property is initialized with the asset you specified at creation time. You may access this property at any time regardless of the current status of the player item.

## See Also

### Getting Information About the Item

var status: WKAudioFilePlayerItemStatus

The status of the player item.

Deprecated

var error: (any Error)?

An error that describes the cause of a failure.

Deprecated

