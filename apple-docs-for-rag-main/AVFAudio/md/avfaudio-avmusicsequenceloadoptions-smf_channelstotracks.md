

- AVFAudio
- AVMusicSequenceLoadOptions
-  smf_ChannelsToTracks 

Type Property

# smf_ChannelsToTracks

An option that represents data on different MIDI channels mapped to multiple tracks.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var smf_ChannelsToTracks: AVMusicSequenceLoadOptions { get }
```

## Discussion

The MIDI sequence contains a tempo track, one track for each MIDI channel in the SMF, and one track (the last track) for `SysEx` and `MetaEvents`.

