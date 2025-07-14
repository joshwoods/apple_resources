

- Audio Toolbox
- Audio File Components
-  Audio File Component Specific Properties 

API Collection

# Audio File Component Specific Properties

## Topics

### Constants

var kAudioFileComponent_AvailableFormatIDs: AudioFilePropertyID

var kAudioFileComponent_AvailableStreamDescriptionsForFormat: AudioFilePropertyID

var kAudioFileComponent_CanRead: AudioFilePropertyID

var kAudioFileComponent_CanWrite: AudioFilePropertyID

var kAudioFileComponent_ExtensionsForType: AudioFilePropertyID

var kAudioFileComponent_FastDispatchTable: AudioFilePropertyID

var kAudioFileComponent_FileTypeName: AudioFilePropertyID

var kAudioFileComponent_HFSTypeCodesForType: AudioFilePropertyID

var kAudioFileComponent_MIMETypesForType: AudioFilePropertyID

var kAudioFileComponent_UTIsForType: AudioFilePropertyID

## See Also

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentGetPropertyProc

typealias AudioFileComponentSetPropertyProc

