

- Core Audio Types
- AudioChannelLayout
-  Audio Channel Layout Tags 

API Collection

# Audio Channel Layout Tags

The identifiers that represent audio channel layouts.

## Overview

Use these values to set the mChannelLayoutTag field of an AudioChannelLayout structure.

## Topics

### General Layouts

var kAudioChannelLayoutTag_UseChannelDescriptions: AudioChannelLayoutTag

An array of audio channel description structures that defines the layout mapping.

var kAudioChannelLayoutTag_UseChannelBitmap: AudioChannelLayoutTag

A bitmap that defines the layout mapping.

var kAudioChannelLayoutTag_Mono: AudioChannelLayoutTag

A standard monophonic stream.

var kAudioChannelLayoutTag_Stereo: AudioChannelLayoutTag

A standard stereophonic stream.

var kAudioChannelLayoutTag_StereoHeadphones: AudioChannelLayoutTag

A standard stereo stream; headphone playback implied.

var kAudioChannelLayoutTag_MatrixStereo: AudioChannelLayoutTag

A matrix-encoded stereo stream.

var kAudioChannelLayoutTag_MidSide: AudioChannelLayoutTag

A middle and side channel audio layout.

var kAudioChannelLayoutTag_XY: AudioChannelLayoutTag

A coincident, angled microphone pair.

var kAudioChannelLayoutTag_Binaural: AudioChannelLayoutTag

A binaural stereo audio layout.

var kAudioChannelLayoutTag_Ambisonic_B_Format: AudioChannelLayoutTag

An ambisonic B-format audio layout.

var kAudioChannelLayoutTag_Quadraphonic: AudioChannelLayoutTag

A quadraphonic audio layout.

var kAudioChannelLayoutTag_Pentagonal: AudioChannelLayoutTag

A pentalgonal audio layout.

var kAudioChannelLayoutTag_Hexagonal: AudioChannelLayoutTag

A hexagonal audio layout.

var kAudioChannelLayoutTag_Octagonal: AudioChannelLayoutTag

An octagonal audio layout.

var kAudioChannelLayoutTag_Cube: AudioChannelLayoutTag

A cubic audio layout.

### Atmos Layouts

var kAudioChannelLayoutTag_Atmos_5_1_2: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Atmos_5_1_4: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Atmos_7_1_2: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Atmos_7_1_4: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Atmos_9_1_6: AudioChannelLayoutTag

### MPEG Defined Layouts

var kAudioChannelLayoutTag_MPEG_1_0: AudioChannelLayoutTag

An MPEG 1-channel audio layout.

var kAudioChannelLayoutTag_MPEG_2_0: AudioChannelLayoutTag

An MPEG 2-channel audio layout.

var kAudioChannelLayoutTag_MPEG_3_0_A: AudioChannelLayoutTag

An MPEG 3-channel, configuration A, audio layout.

var kAudioChannelLayoutTag_MPEG_3_0_B: AudioChannelLayoutTag

An MPEG 3-channel, configuration B, audio layout.

var kAudioChannelLayoutTag_MPEG_4_0_A: AudioChannelLayoutTag

An MPEG 4-channel, configuration A, audio layout.

var kAudioChannelLayoutTag_MPEG_4_0_B: AudioChannelLayoutTag

An MPEG 4-channel, configuration B, audio layout

var kAudioChannelLayoutTag_MPEG_5_0_A: AudioChannelLayoutTag

An MPEG 5-channel, configuration A, audio layout.

var kAudioChannelLayoutTag_MPEG_5_0_B: AudioChannelLayoutTag

An MPEG 5-channel, configuration B, audio layout.

var kAudioChannelLayoutTag_MPEG_5_0_C: AudioChannelLayoutTag

An MPEG 5-channel, configuration C, audio layout.

var kAudioChannelLayoutTag_MPEG_5_0_D: AudioChannelLayoutTag

An MPEG 5-channel, configuration D, audio layout.

var kAudioChannelLayoutTag_MPEG_5_0_E: AudioChannelLayoutTag

5 channels, L R Rls Rrs C

var kAudioChannelLayoutTag_MPEG_5_1_A: AudioChannelLayoutTag

An MPEG 5.1-channel, configuration A, audio layout.

var kAudioChannelLayoutTag_MPEG_5_1_B: AudioChannelLayoutTag

An MPEG 5.1-channel, configuration B, audio layout.

var kAudioChannelLayoutTag_MPEG_5_1_C: AudioChannelLayoutTag

An MPEG 5.1-channel, configuration C, audio layout.

var kAudioChannelLayoutTag_MPEG_5_1_D: AudioChannelLayoutTag

An MPEG 5.1-channel, configuration D, audio layout.

var kAudioChannelLayoutTag_MPEG_5_1_E: AudioChannelLayoutTag

6 channels, L R Rls Rrs C LFE

var kAudioChannelLayoutTag_MPEG_6_1_A: AudioChannelLayoutTag

An MPEG 6.1-channel, configuration A, audio layout.

var kAudioChannelLayoutTag_MPEG_6_1_B: AudioChannelLayoutTag

7 channels, L R Ls Rs C Cs LFE

var kAudioChannelLayoutTag_MPEG_7_1_A: AudioChannelLayoutTag

An MPEG 7.1-channel, configuration A, audio layout.

var kAudioChannelLayoutTag_MPEG_7_1_B: AudioChannelLayoutTag

An MPEG 7.1-channel, configuration B, audio layout.

var kAudioChannelLayoutTag_MPEG_7_1_C: AudioChannelLayoutTag

An MPEG 7.1-channel, configuration C, audio layout.

var kAudioChannelLayoutTag_MPEG_7_1_D: AudioChannelLayoutTag

8 channels, L R Rls Rrs Ls Rs C LFE

var kAudioChannelLayoutTag_Emagic_Default_7_1: AudioChannelLayoutTag

An Emagic 7.1-channel default audio layout.

var kAudioChannelLayoutTag_SMPTE_DTV: AudioChannelLayoutTag

An SMPTE DTV audio layout.

### CICP

var kAudioChannelLayoutTag_CICP_1: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_2: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_3: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_4: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_5: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_6: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_7: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_9: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_10: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_11: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_12: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_13: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_14: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_15: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_16: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_17: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_18: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_19: AudioChannelLayoutTag

var kAudioChannelLayoutTag_CICP_20: AudioChannelLayoutTag

### ITU Defined Layouts

var kAudioChannelLayoutTag_ITU_1_0: AudioChannelLayoutTag

An ITU 1-channel audio layout.

var kAudioChannelLayoutTag_ITU_2_0: AudioChannelLayoutTag

An ITU 2-channel audio layout.

var kAudioChannelLayoutTag_ITU_2_1: AudioChannelLayoutTag

An ITU 2.1-channel audio layout.

var kAudioChannelLayoutTag_ITU_2_2: AudioChannelLayoutTag

An ITU 2.2-channel audio layout.

var kAudioChannelLayoutTag_ITU_3_0: AudioChannelLayoutTag

An ITU 3-channel audio layout.

var kAudioChannelLayoutTag_ITU_3_1: AudioChannelLayoutTag

An ITU 3.1-channel audio layout.

var kAudioChannelLayoutTag_ITU_3_2: AudioChannelLayoutTag

An ITU 3.2-channel audio layout.

var kAudioChannelLayoutTag_ITU_3_2_1: AudioChannelLayoutTag

An ITU 3.2.1-channel audio layout.

var kAudioChannelLayoutTag_ITU_3_4_1: AudioChannelLayoutTag

An ITU 3.4.1-channel audio layout.

### DVD Defined Layouts

var kAudioChannelLayoutTag_DVD_0: AudioChannelLayoutTag

A DVD monaural audio layout.

var kAudioChannelLayoutTag_DVD_1: AudioChannelLayoutTag

A DVD stereo audio layout.

var kAudioChannelLayoutTag_DVD_2: AudioChannelLayoutTag

A DVD 3-channel audio layout.

var kAudioChannelLayoutTag_DVD_3: AudioChannelLayoutTag

A DVD 4-channel audio layout.

var kAudioChannelLayoutTag_DVD_4: AudioChannelLayoutTag

A DVD 2.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_5: AudioChannelLayoutTag

A DVD 3.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_6: AudioChannelLayoutTag

A DVD 4.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_7: AudioChannelLayoutTag

A DVD 3-channel audio layout.

var kAudioChannelLayoutTag_DVD_8: AudioChannelLayoutTag

A DVD 4-channel audio layout.

var kAudioChannelLayoutTag_DVD_9: AudioChannelLayoutTag

A DVD 5-channel audio layout.

var kAudioChannelLayoutTag_DVD_10: AudioChannelLayoutTag

A DVD 3.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_11: AudioChannelLayoutTag

A DVD 4.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_12: AudioChannelLayoutTag

A DVD 5.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_13: AudioChannelLayoutTag

A DVD 4-channel audio layout.

var kAudioChannelLayoutTag_DVD_14: AudioChannelLayoutTag

A DVD 5-channel audio layout.

var kAudioChannelLayoutTag_DVD_15: AudioChannelLayoutTag

A DVD 3.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_16: AudioChannelLayoutTag

A DVD 4.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_17: AudioChannelLayoutTag

A DVD 5.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_18: AudioChannelLayoutTag

A DVD 4.1-channel audio layout.

var kAudioChannelLayoutTag_DVD_19: AudioChannelLayoutTag

A DVD 5-channel audio layout.

var kAudioChannelLayoutTag_DVD_20: AudioChannelLayoutTag

A DVD 5.1-channel audio layout.

### Symmetrical Layouts

var kAudioChannelLayoutTag_AudioUnit_4: AudioChannelLayoutTag

A quadraphonic symmetrical layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_5: AudioChannelLayoutTag

A pentagonal symmetrical layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_6: AudioChannelLayoutTag

A hexagonal symmetrical layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_8: AudioChannelLayoutTag

An octagonal symmetrical layout, recommended for use by audio units.

### Surround Based Layouts

var kAudioChannelLayoutTag_AudioUnit_5_0: AudioChannelLayoutTag

A 5-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_6_0: AudioChannelLayoutTag

A 6-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_7_0: AudioChannelLayoutTag

A 7-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_7_0_Front: AudioChannelLayoutTag

An alternate 7-channel surround-based layout, for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_5_1: AudioChannelLayoutTag

A 5.1-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_6_1: AudioChannelLayoutTag

A 6.1-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_7_1: AudioChannelLayoutTag

A 7.1-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_AudioUnit_7_1_Front: AudioChannelLayoutTag

A 7.1-channel surround-based layout, recommended for use by audio units.

var kAudioChannelLayoutTag_TMH_10_2_std: AudioChannelLayoutTag

A TMH 10.2 multiple-channel surround-based layout .

var kAudioChannelLayoutTag_TMH_10_2_full: AudioChannelLayoutTag

An extended TMH 10.2 multiple-channel surround-based layout, recommended for use by audio units.

### AAC Defined Layouts

var kAudioChannelLayoutTag_AAC_3_0: AudioChannelLayoutTag

An AAC 3-channel audio layout.

var kAudioChannelLayoutTag_AAC_Quadraphonic: AudioChannelLayoutTag

An AAC quadraphonic surround-based layout.

var kAudioChannelLayoutTag_AAC_4_0: AudioChannelLayoutTag

An AAC 4-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_5_0: AudioChannelLayoutTag

An AAC 5-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_5_1: AudioChannelLayoutTag

An AAC 5.1-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_6_0: AudioChannelLayoutTag

An AAC 6-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_6_1: AudioChannelLayoutTag

An AAC 6.1-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_7_0: AudioChannelLayoutTag

An AAC 7-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_7_1: AudioChannelLayoutTag

An AAC 7.1-channel surround-based layout.

var kAudioChannelLayoutTag_AAC_7_1_B: AudioChannelLayoutTag

An AAC 7.1-channel, configuration B, surround-based layout.

var kAudioChannelLayoutTag_AAC_7_1_C: AudioChannelLayoutTag

An AAC 7.1-channel, configuration C, surround-based layout.

var kAudioChannelLayoutTag_AAC_Octagonal: AudioChannelLayoutTag

An AAC 8-channel surround-based layout.

### AC3 Defined Layouts

var kAudioChannelLayoutTag_AC3_1_0_1: AudioChannelLayoutTag

An AC-3 layout.

var kAudioChannelLayoutTag_AC3_3_0: AudioChannelLayoutTag

An AC-3 layout.

var kAudioChannelLayoutTag_AC3_3_1: AudioChannelLayoutTag

An AC-3 layout.

var kAudioChannelLayoutTag_AC3_3_0_1: AudioChannelLayoutTag

An AC-3 layout.

var kAudioChannelLayoutTag_AC3_2_1_1: AudioChannelLayoutTag

An AC-3 layout.

var kAudioChannelLayoutTag_AC3_3_1_1: AudioChannelLayoutTag

An AC-3 layout.

### EAC3 Defined Layouts

var kAudioChannelLayoutTag_EAC_6_0_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC_7_0_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_6_1_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_6_1_B: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_6_1_C: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_B: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_C: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_D: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_E: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_F: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_G: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

var kAudioChannelLayoutTag_EAC3_7_1_H: AudioChannelLayoutTag

A Blu-ray Disc audio layout for Enhanced AC-3, also known as Dolby Digital Plus.

### DTS Defined Layouts

var kAudioChannelLayoutTag_DTS_3_1: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_4_1: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_0_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_0_B: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_0_C: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_1_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_1_B: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_1_C: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_6_1_D: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_7_0: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_7_1: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_8_0_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_8_0_B: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_8_1_A: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

var kAudioChannelLayoutTag_DTS_8_1_B: AudioChannelLayoutTag

A Blu-ray Disc audio layout, defined by DTS (Digital Theater Systems Ltd.).

### HOA Defined Layouts

var kAudioChannelLayoutTag_HOA_ACN_N3D: AudioChannelLayoutTag

A Higher-order Ambisonics, full 3D normalization audio layout.

var kAudioChannelLayoutTag_HOA_ACN_SN3D: AudioChannelLayoutTag

A Higher-order Ambisonics, Schmidt semi-normalization audio layout.

### General Information Tags

var kAudioChannelLayoutTag_DiscreteInOrder: AudioChannelLayoutTag

A tag used to map input channels to output channels without changing the channel order.

var kAudioChannelLayoutTag_Unknown: AudioChannelLayoutTag

The channel layout is unknown.

### Reserved Tag Range

The tags in this section define a range of values reserved for future Apple use. Do not create tags in this range.

var kAudioChannelLayoutTag_BeginReserved: AudioChannelLayoutTag

The beginning value for a reserved range of layout tags.

var kAudioChannelLayoutTag_EndReserved: AudioChannelLayoutTag

The ending value for a reserved range of layout tags.

### Wave Layouts

var kAudioChannelLayoutTag_WAVE_2_1: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_3_0: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_4_0_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_4_0_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_5_0_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_5_0_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_5_1_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_5_1_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_6_1: AudioChannelLayoutTag

var kAudioChannelLayoutTag_WAVE_7_1: AudioChannelLayoutTag

### Logic Pro Layouts

var kAudioChannelLayoutTag_Logic_4_0_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_4_0_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_4_0_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_0_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_0_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_0_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_0_D: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_1_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_1_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_1_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_5_1_D: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_0_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_0_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_0_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_1_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_1_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_1_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_6_1_D: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_7_1_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_7_1_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_7_1_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_7_1_SDDS_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_7_1_SDDS_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_7_1_SDDS_C: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Atmos_5_1_2: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Atmos_5_1_4: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Atmos_7_1_2: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Atmos_7_1_4_A: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Atmos_7_1_4_B: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Atmos_7_1_6: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Mono: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Quadraphonic: AudioChannelLayoutTag

var kAudioChannelLayoutTag_Logic_Stereo: AudioChannelLayoutTag

## See Also

### Accessing the Data

var mChannelBitmap: AudioChannelBitmap

If `mChannelLayoutTag` is set to `kAudioChannelLayoutTag_UseChannelBitmap`, this field is the channel-use bitmap.

struct AudioChannelBitmap

The supported channel bitmaps to use when defining channel layouts.

var mChannelDescriptions: AudioChannelDescription

A variable length array of `mNumberChannelDescription` elements that describes a layout. If the `mChannelLayoutTag` field is set to `kAudioChannelLayoutTag_UseChannelDescriptions`, use this field to describe the layout.

var mChannelLayoutTag: AudioChannelLayoutTag

The `AudioChannelLayoutTag` value that indicates the layout. See Audio Channel Layout Tags for possible values.

typealias AudioChannelLayoutTag

Identifies a previously-defined channel layout.

var mNumberChannelDescriptions: UInt32

The number of items in the `mChannelDescriptions` array.

func AudioChannelLayoutTag_GetNumberOfChannels(AudioChannelLayoutTag) -> UInt32

Retrieves the number of channels from an audio channel layout tag.

