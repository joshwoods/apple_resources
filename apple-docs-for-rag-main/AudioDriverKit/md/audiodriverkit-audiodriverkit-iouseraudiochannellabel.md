

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioChannelLabel 

Enumeration

# IOUserAudioChannelLabel

Constants to set the preferred channel layout on an audio device.

DriverKit 21.0+

``` source
enum IOUserAudioChannelLabel : uint32_t;
```

## Discussion

These channel labels attempt to list all labels in common use. Due to the ambiguities in channel labeling by various groups, there may be some overlap or duplication in the labels below. Use the label which most clearly describes what you mean.

## Topics

### Left Channels

Left

The left channel.

LeftCenter

The left center channel.

LeftTopFront

The left top front channel.

VerticalHeightLeft

A synonym for the top-left–front channel.

LeftTopMiddle

The left top middle channel.

LeftTopRear

The left top rear channel.

LeftTotal

A matrix encode of four left channels.

LeftWide

The left wide channel.

### Right Channels

Right

The right channel.

RightCenter

The right center channel.

RightTopFront

The right top front channel.

VerticalHeightRight

A synonym for the top-right–front channel.

RightTopMiddle

The right top middle channel.

RightTopRear

The right top rear channel.

RightTotal

A matrix encode of four right channels.

RightWide

The right wide channel.

### Center Channels

Center

The center channel.

CenterTopFront

The center top front channel.

VerticalHeightCenter

A synonym for the top-center–front channel.

CenterTopMiddle

The center top middle channel.

CenterTopRear

The center top rear channel.

### Back Channels

TopBackCenter

The top-rear–center channel.

TopCenterSurround

A synonym for the top-rear–center channel.

TopBackLeft

The top-rear–left channel.

TopBackRight

The top-rear–right channel.

### Surround Channels

CenterSurround

The center surround channel.

CenterSurroundDirect

The center surround direct channel.

LeftSurround

The left surround channel.

LeftSurroundDirect

The left surround direct channel.

RearSurroundLeft

The rear left surround channel.

RearSurroundRight

The right rear surround channel.

RightSurround

The right surround channel.

RightSurroundDirect

The right surround direct channel.

### Low-Frequency Effects Channels

LFE2

The low-frequency effects 2 (LFE2) channel.

LFEScreen

The low-frequency effects (LFE) screen channel.

### Monaural Channels

Mono

The mono channel.

### Alternate Content Channels

ClickTrack

The click track channel.

DialogCentricMix

The dialog-centric mix channel.

ForeignLanguage

The foreign language channel.

HearingImpaired

The audio for the hearing-impaired channel.

Haptic

The haptic effects channel.

Narration

The narration channel.

### Mid/Side Recording

MS_Mid

The Mid/Side recording mid channel.

MS_Side

The Mid/Side recording side channel.

### X/Y Recording Channels

XY_X

The X/Y recording X channel.

XY_Y

The X/Y recording Y channel.

### First-Order Ambisonic Channels

Ambisonic_W

The ambisonic W channel.

Ambisonic_X

The ambisonic X channel.

Ambisonic_Y

The ambisonic Y channel.

Ambisonic_Z

The ambisonic Z channel.

### Binaural Recording

BinauralLeft

The binaural left channel.

BinauralRight

The binaural right channel.

### Headphone Channels

HeadphonesLeft

The left headphone channel.

HeadphonesRight

The right headphone channel.

### Unnumbered Discrete Channels

Discrete

A generic discrete channel.

### Numbered Discrete Channels

Discrete_0

Numbered discrete channel 0.

Discrete_1

Numbered discrete channel 1.

Discrete_2

Numbered discrete channel 2.

Discrete_3

Numbered discrete channel 3.

Discrete_4

Numbered discrete channel 4.

Discrete_5

Numbered discrete channel 5.

Discrete_6

Numbered discrete channel 6.

Discrete_7

Numbered discrete channel 7.

Discrete_8

Numbered discrete channel 8.

Discrete_9

Numbered discrete channel 9.

Discrete_10

Numbered discrete channel 10.

Discrete_11

Numbered discrete channel 11.

Discrete_12

Numbered discrete channel 12.

Discrete_13

Numbered discrete channel 13.

Discrete_14

Numbered discrete channel 14.

Discrete_15

Numbered discrete channel 15.

Discrete_65535

The maximum numbered discrete channel.

### Generic High Order Ambisonics ACN Channel

HOA_ACN

A generic high order ambisonics (HOA) Ambisonic Channel Number (ACN).

### Numbered High Order Ambisonics ACN Channels

HOA_ACN_0

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 0.

HOA_ACN_1

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 1.

HOA_ACN_2

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 2.

HOA_ACN_3

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 3.

HOA_ACN_4

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 4.

HOA_ACN_5

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 5.

HOA_ACN_6

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 6.

HOA_ACN_7

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 7.

HOA_ACN_8

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 8.

HOA_ACN_9

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 9.

HOA_ACN_10

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 10

HOA_ACN_11

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 11.

HOA_ACN_12

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 12.

HOA_ACN_13

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 13.

HOA_ACN_14

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 14.

HOA_ACN_15

Numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN) 15.

HOA_ACN_65024

The maximum numbered high order ambisonics (HOA) Ambisonic Channel Number (ACN).

### Special Values

Unused

An unknown or otherwise unspecified channel use.

UseCoordinates

A channel that uses coodinates to describe its position.

### Reserved Values

BeginReserved

The beginning of the range of channel values reserved for internal use.

EndReserved

### Enumeration Cases

Unknown

unknown or unspecified other use

## See Also

### Working with Channel Layouts

SetPreferredChannelsForStereo

Sets the channel indices for the prefered stereo pair.

GetPreferredChannelsForStereo

Returns the channel indices for the prefered stereo pair.

SetPreferredInputChannelLayout

Sets the input channel layout, using an array of audio channel label values.

SetPreferredOutputChannelLayout

Sets the output channel layout, using an array of audio channel label values.

