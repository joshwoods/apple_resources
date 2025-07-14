

- WatchKit
- WKAudioFilePlayer
-  rate Deprecated

Instance Property

# rate

The current rate of playback.

watchOS 2.0–6.0Deprecated

``` source
var rate: Float { get set }
```

## Discussion

The playback rate refers to the playback speed. A value of `0.0` indicates that playback is paused while a value of `1.0` indicates playback is proceeding at the natural rate of the item. Rates other than `0.0` and `1.0` let you play the audio faster or slower than the natural rate of the item. Negative values let you play the audio in reverse.

## See Also

### Configuring and Controlling Playback

func play()

Begins playback of the current item.

Deprecated

func pause()

Pauses playback of the associated item.

Deprecated

