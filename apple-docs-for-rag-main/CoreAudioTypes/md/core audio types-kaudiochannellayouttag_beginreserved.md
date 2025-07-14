

- Core Audio Types
-  kAudioChannelLayoutTag_BeginReserved 

Global Variable

# kAudioChannelLayoutTag_BeginReserved

The beginning value for a reserved range of layout tags.

iOS 12.0+iPadOS 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var kAudioChannelLayoutTag_BeginReserved: AudioChannelLayoutTag { get }
```

## Discussion

The values in the range between `kAudioChannelLayoutTag_BeginReserved` and kAudioChannelLayoutTag_EndReserved are for future Apple use. Do not create layout tags that fall in the range created by these values.

## See Also

### Reserved Tag Range

var kAudioChannelLayoutTag_EndReserved: AudioChannelLayoutTag

The ending value for a reserved range of layout tags.

