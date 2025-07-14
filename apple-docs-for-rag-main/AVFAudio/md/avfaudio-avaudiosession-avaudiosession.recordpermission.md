

- AVFAudio
- AVAudioSession
-  AVAudioSession.RecordPermission 

Enumeration

# AVAudioSession.RecordPermission

The values that define the current state of the record permission request.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum RecordPermission
```

## Overview

The recordPermission property returns these values.

## Topics

### Record Permissions

case undetermined

A value that indicates that the user hasn’t granted or denied recording permission.

Deprecated

case denied

A value that indicates that the user has denied recording permission.

Deprecated

case granted

A value that indicates that the user has granted recording permission.

Deprecated

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

