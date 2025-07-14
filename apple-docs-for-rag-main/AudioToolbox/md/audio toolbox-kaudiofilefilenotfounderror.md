

- Audio Toolbox
-  kAudioFileFileNotFoundError 

Global Variable

# kAudioFileFileNotFoundError

File not found.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFileFileNotFoundError: OSStatus { get }
```

## See Also

### Result Codes

var kAudioFileUnspecifiedError: OSStatus

An unspecified error has occurred.

var kAudioFileUnsupportedFileTypeError: OSStatus

The file type is not supported.

var kAudioFileUnsupportedDataFormatError: OSStatus

The data format is not supported by this file type.

var kAudioFileUnsupportedPropertyError: OSStatus

The property is not supported.

var kAudioFileBadPropertySizeError: OSStatus

The size of the property data was not correct.

var kAudioFilePermissionsError: OSStatus

The operation violated the file permissions. For example, an attempt was made to write to a file opened with the `kAudioFileReadPermission` constant.

var kAudioFileNotOptimizedError: OSStatus

The chunks following the audio data chunk are preventing the extension of the audio data chunk. To write more data, you must optimize the file.

var kAudioFileInvalidChunkError: OSStatus

Either the chunk does not exist in the file or it is not supported by the file.

var kAudioFileDoesNotAllow64BitDataSizeError: OSStatus

The file offset was too large for the file type. The AIFF and WAVE file format types have 32-bit file size limits.

var kAudioFileInvalidPacketOffsetError: OSStatus

A packet offset was past the end of the file, or not at the end of the file when a VBR format was written, or a corrupt packet size was read when the packet table was built.

var kAudioFileInvalidFileError: OSStatus

The file is malformed, or otherwise not a valid instance of an audio file of its type.

var kAudioFileOperationNotSupportedError: OSStatus

The operation cannot be performed.

var kAudioFileNotOpenError: OSStatus

The file is closed.

var kAudioFileEndOfFileError: OSStatus

End of file.

var kAudioFilePositionError: OSStatus

Invalid file position.

