

- Audio Toolbox
- AudioFileFlags
-  dontPageAlignAudioData 

Type Property

# dontPageAlignAudioData

Typically, the audio data in a file is page aligned. To make reading the file data as fast as possible, you can use page-aligned data to take advantage of optimized code paths in the file system. However, when space is at a premium, you might want to avoid the additional padding required to attain alignment. To do so, set this flag when calling AudioFileCreate or AudioFileCreateWithURL(_:_:_:_:_:).

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var dontPageAlignAudioData: AudioFileFlags { get }
```

## See Also

### Flags

static var eraseFile: AudioFileFlags

