

- Core Services
- File Metadata
- MDItem
- Audio Metadata Attribute Keys
-  kMDItemAudioChannelCount 

Global Variable

# kMDItemAudioChannelCount

Number of channels in the audio data contained in the file. A CFNumber.

macOS 10.4+

``` source
let kMDItemAudioChannelCount: CFString!
```

## Discussion

This integer value only represents the number of discreet channels of audio data found in the file. It does not indicate any configuration of the data in regards to a user's speaker setup.

