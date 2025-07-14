

- Audio Toolbox
-  kAudioFileStreamError_NotOptimized 

Global Variable

# kAudioFileStreamError_NotOptimized

It is not possible to produce output packets because the streamed audio file’s packet table or other defining information is not present or appears after the audio data.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFileStreamError_NotOptimized: OSStatus { get }
```

## See Also

### Result Codes

Audio File Errors

var kAudioFileStreamError_UnsupportedFileType: OSStatus

The specified file type is not supported.

var kAudioFileStreamError_UnsupportedDataFormat: OSStatus

The data format is not supported by the specified file type.

var kAudioFileStreamError_UnsupportedProperty: OSStatus

The property is not supported.

var kAudioFileStreamError_BadPropertySize: OSStatus

The size of the buffer you provided for property data was not correct.

var kAudioFileStreamError_InvalidPacketOffset: OSStatus

A packet offset was less than `0`, or past the end of the file, or a corrupt packet size was read when building the packet table.

var kAudioFileStreamError_InvalidFile: OSStatus

The file is malformed, not a valid instance of an audio file of its type, or not recognized as an audio file.

var kAudioFileStreamError_ValueUnknown: OSStatus

The property value is not present in this file before the audio data.

var kAudioFileStreamError_DataUnavailable: OSStatus

The amount of data provided to the parser was insufficient to produce any result.

var kAudioFileStreamError_IllegalOperation: OSStatus

An illegal operation was attempted.

var kAudioFileStreamError_UnspecifiedError: OSStatus

An unspecified error has occurred.

var kAudioFileStreamError_DiscontinuityCantRecover: OSStatus

A discontinuity has occurred in the audio data, and Audio File Stream Services cannot recover.

