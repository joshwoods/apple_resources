

- Audio Toolbox
- Audio File Stream Services
-  Audio File Errors 

API Collection

# Audio File Errors

## Topics

### Constants

var kAudioFileBadPropertySizeError: OSStatus

The size of the property data was not correct.

var kAudioFileDoesNotAllow64BitDataSizeError: OSStatus

The file offset was too large for the file type. The AIFF and WAVE file format types have 32-bit file size limits.

var kAudioFileEndOfFileError: OSStatus

End of file.

var kAudioFileFileNotFoundError: OSStatus

File not found.

var kAudioFileInvalidChunkError: OSStatus

Either the chunk does not exist in the file or it is not supported by the file.

var kAudioFileInvalidFileError: OSStatus

The file is malformed, or otherwise not a valid instance of an audio file of its type.

var kAudioFileInvalidPacketOffsetError: OSStatus

A packet offset was past the end of the file, or not at the end of the file when a VBR format was written, or a corrupt packet size was read when the packet table was built.

var kAudioFileNotOpenError: OSStatus

The file is closed.

var kAudioFileNotOptimizedError: OSStatus

The chunks following the audio data chunk are preventing the extension of the audio data chunk. To write more data, you must optimize the file.

var kAudioFileOperationNotSupportedError: OSStatus

The operation cannot be performed.

var kAudioFilePermissionsError: OSStatus

The operation violated the file permissions. For example, an attempt was made to write to a file opened with the `kAudioFileReadPermission` constant.

var kAudioFilePositionError: OSStatus

Invalid file position.

var kAudioFileUnspecifiedError: OSStatus

An unspecified error has occurred.

var kAudioFileUnsupportedDataFormatError: OSStatus

The data format is not supported by this file type.

var kAudioFileUnsupportedFileTypeError: OSStatus

The file type is not supported.

var kAudioFileUnsupportedPropertyError: OSStatus

The property is not supported.

var kAudioFileInvalidPacketDependencyError: OSStatus

## See Also

### Result Codes

var kAudioFileStreamError_UnsupportedFileType: OSStatus

The specified file type is not supported.

var kAudioFileStreamError_UnsupportedDataFormat: OSStatus

The data format is not supported by the specified file type.

var kAudioFileStreamError_UnsupportedProperty: OSStatus

The property is not supported.

var kAudioFileStreamError_BadPropertySize: OSStatus

The size of the buffer you provided for property data was not correct.

var kAudioFileStreamError_NotOptimized: OSStatus

It is not possible to produce output packets because the streamed audio file’s packet table or other defining information is not present or appears after the audio data.

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

