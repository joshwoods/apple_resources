

- Audio Toolbox
- MusicSequenceLoadFlags
-  smf_ChannelsToTracks 

Type Property

# smf_ChannelsToTracks

If this flag is set the resultant Sequence will contain a tempo track, 1 track for each MIDI Channel that is found in the SMF, 1 track for SysEx or MetaEvents - and this will be the last track in the sequence after the LoadSMFWithFlags calls.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var smf_ChannelsToTracks: MusicSequenceLoadFlags { get }
```

