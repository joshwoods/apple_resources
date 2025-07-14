

- Audio Toolbox
- Audio File Stream Services
-  Audio File Stream Flags 

API Collection

# Audio File Stream Flags

Flags set by the property listener callback and the AudioFileStreamParseBytes(_:_:_:_:) function.

## Topics

### Constants

static var propertyIsCached: AudioFileStreamPropertyFlags

This flag is set when the callback AudioFileStream_PropertyListenerProc is invoked in the case that the value of the property has been cached and can be obtained later.

static var cacheProperty: AudioFileStreamPropertyFlags

A property listener sets this flag to instruct the parser to cache the property value so that it remains available after the callback returns.

static var discontinuity: AudioFileStreamParseFlags

Pass this flag to the AudioFileStreamParseBytes(_:_:_:_:) function to signal a discontinuity in the audio data.

static var offsetIsEstimated: AudioFileStreamSeekFlags

This flag is returned by the AudioFileStreamSeek(_:_:_:_:) function if the byte offset is only an estimate.

## See Also

### Constants

Audio File Stream Properties

Audio file stream properties contain information that you can use to help interpret the audio data in a stream.

