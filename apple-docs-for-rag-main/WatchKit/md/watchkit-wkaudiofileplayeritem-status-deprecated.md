

- WatchKit
- WKAudioFilePlayerItem
-  status Deprecated

Instance Property

# status

The status of the player item.

watchOS 2.0–6.0Deprecated

``` source
var status: WKAudioFilePlayerItemStatus { get }
```

## Discussion

When the value of this property is WKAudioFilePlayerItemStatus.failed, the error property contains the reason for the failure.

## See Also

### Getting Information About the Item

var asset: WKAudioFileAsset

The audio file asset being managed.

Deprecated

var error: (any Error)?

An error that describes the cause of a failure.

Deprecated

