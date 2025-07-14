

- Core Audio
-  AudioHardwareObject 

Class

# AudioHardwareObject

macOS 15.0+

``` source
class AudioHardwareObject
```

## Topics

### Initializers

init(id: AudioObjectID)

### Instance Properties

var baseClassID: AudioClassID

var classID: AudioClassID

var creatorBundleID: String

var delegates: [any PropertyListenerDelegate]

var firmwareVersion: String

let id: AudioObjectID

var isIdentifying: Bool

var manufacturer: String

var modelName: String

var name: String

var ownedObjects: [AudioHardwareObject]

var owner: AudioHardwareObject?

var serialNumber: String

### Instance Methods

func addListener(forProperties: [AudioObjectPropertyAddress], dispatchQueue: dispatch_queue_t?) throws

func hasProperty(address: AudioObjectPropertyAddress) -> Bool

func isPropertySettable(address: AudioObjectPropertyAddress) throws -> Bool

func propertyData(address: AudioObjectPropertyAddress, qualifier: Data?) throws -> Data

func propertyDataSize(address: AudioObjectPropertyAddress, qualifier: Data?) throws -> Int

func removeListener(forProperties: [AudioObjectPropertyAddress], dispatchQueue: dispatch_queue_t?) throws

func setCreatorBundleID(String) throws

func setIsIdentifying(Bool) throws

func setName(String) throws

func setPropertyData(address: AudioObjectPropertyAddress, qualifier: Data?, data: Data) throws

func setPropertyData(address: AudioObjectPropertyAddress, qualifier: Data?, data: inout Data) async throws

## Relationships

### Inherited By

- AudioHardwareBox
- AudioHardwareClock
- AudioHardwareControl
- AudioHardwarePlugin
- AudioHardwareProcess
- AudioHardwareStream
- AudioHardwareSystem
- AudioHardwareTap

