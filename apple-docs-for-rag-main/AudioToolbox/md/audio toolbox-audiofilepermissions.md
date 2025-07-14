

- Audio Toolbox
-  AudioFilePermissions 

Enumeration

# AudioFilePermissions

Flags for use when opening an audio file.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum AudioFilePermissions
```

## Overview

Use these flags with the AudioFileOpenURL(_:_:_:_:) and AudioFileOpen functions.

## Topics

### Constants

case readPermission

File is read-only.

case readWritePermission

File has read-write permission.

case writePermission

File is write-only.

### Initializers

init?(rawValue: Int8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

struct AudioBytePacketTranslationFlags

struct AudioFileFlags

struct AudioFileRegionFlags

Flags that specify a playback direction for an audio file region structure.

struct AudioFileStreamParseFlags

struct AudioFileStreamPropertyFlags

struct AudioFileStreamSeekFlags

