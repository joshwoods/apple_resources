

- Core Audio Types
-  kAudioChannelLayoutTag_HOA_ACN_N3D 

Global Variable

# kAudioChannelLayoutTag_HOA_ACN_N3D

A Higher-order Ambisonics, full 3D normalization audio layout.

iOS 11.0+iPadOS 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var kAudioChannelLayoutTag_HOA_ACN_N3D: AudioChannelLayoutTag { get }
```

## Discussion

This tag needs to be `ORed` with the number of HOA components, not the HOA order.

## See Also

### HOA Defined Layouts

var kAudioChannelLayoutTag_HOA_ACN_SN3D: AudioChannelLayoutTag

A Higher-order Ambisonics, Schmidt semi-normalization audio layout.

