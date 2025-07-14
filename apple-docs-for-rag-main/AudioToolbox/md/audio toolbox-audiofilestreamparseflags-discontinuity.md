

- Audio Toolbox
- AudioFileStreamParseFlags
-  discontinuity 

Type Property

# discontinuity

Pass this flag to the AudioFileStreamParseBytes(_:_:_:_:) function to signal a discontinuity in the audio data.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var discontinuity: AudioFileStreamParseFlags { get }
```

## Discussion

Any partial packet straddling a buffer boundary is discarded to avoid having the parser call your callback with a corrupt packet. After a discontinuity occurs, the AudioFileStreamSeek(_:_:_:_:) function might return approximate values for some data formats.

