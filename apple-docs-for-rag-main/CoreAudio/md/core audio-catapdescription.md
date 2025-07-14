

- Core Audio
-  CATapDescription 

Class

# CATapDescription

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class CATapDescription
```

## Topics

### Initializers

init()

convenience init(excludingProcesses: [AudioObjectID], deviceUID: String, stream: UInt)

convenience init(monoGlobalTapButExcludeProcesses: [AudioObjectID])

convenience init(monoMixdownOfProcesses: [AudioObjectID])

convenience init(processes: [AudioObjectID], deviceUID: String, stream: UInt)

convenience init(stereoGlobalTapButExcludeProcesses: [AudioObjectID])

convenience init(stereoMixdownOfProcesses: [AudioObjectID])

### Instance Properties

var deviceUID: String?

var isExclusive: Bool

var isMixdown: Bool

var isMono: Bool

var isPrivate: Bool

var muteBehavior: CATapMuteBehavior

var name: String

var processes: [AudioObjectID]

var stream: UInt?

var uuid: UUID

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

