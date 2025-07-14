

- AVFoundation
- AVPlayer
-  preventsDisplaySleepDuringVideoPlayback 

Instance Property

# preventsDisplaySleepDuringVideoPlayback

A Boolean value that indicates whether video playback prevents display and device sleep.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+

``` source
nonisolated
var preventsDisplaySleepDuringVideoPlayback: Bool { get set }
```

## Discussion

The default value is true in iOS, tvOS and Mac Catalyst apps, and false in macOS.

Setting this property to false doesn’t force the display to sleep, it only stops preventing display sleep. Other apps, or frameworks within your app may still prevent display sleep for various reasons.

Note

Before macOS 13, iOS 16, tvOS 16, and watchOS 9, you can only access this property from the main thread or queue.

## See Also

### Preventing Sleep and Backgrounding

var preventsAutomaticBackgroundingDuringVideoPlayback: Bool

A Boolean value that indicates whether video playback prevents the system from automatically backgrounding the app.

