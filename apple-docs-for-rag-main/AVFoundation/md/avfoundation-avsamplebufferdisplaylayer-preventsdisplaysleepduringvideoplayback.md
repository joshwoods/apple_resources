

- AVFoundation
- AVSampleBufferDisplayLayer
-  preventsDisplaySleepDuringVideoPlayback 

Instance Property

# preventsDisplaySleepDuringVideoPlayback

A Boolean value that indicates whether the layer prevents the system from sleeping during video playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+

``` source
var preventsDisplaySleepDuringVideoPlayback: Bool { get set }
```

## Discussion

Setting this property to false doesn’t force the display to sleep; it only stops preventing display sleep. Other apps or frameworks within your app may still be preventing display sleep for various reasons.

The default value is true in iOS, tvOS, and Mac Catalyst. The default value in macOS is false.

Note

If you enqueue sample buffers for playback at the user’s request, you should ensure that you set the value of this property to true. If your app isn’t displaying video as part of the user’s primary focus, set the value of this property to false.

## See Also

### Preventing backgrounding

var preventsAutomaticBackgroundingDuringVideoPlayback: Bool

A Boolean value that indicates whether video playback prevents the system from automatically backgrounding an app.

