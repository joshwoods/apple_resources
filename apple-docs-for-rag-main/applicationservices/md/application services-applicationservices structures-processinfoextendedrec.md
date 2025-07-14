

- Application Services
- ApplicationServices Structures
-  ProcessInfoExtendedRec 

Structure

# ProcessInfoExtendedRec

macOS 10.0+

``` source
struct ProcessInfoExtendedRec
```

## Topics

### Initializers

init()

init(processInfoLength: UInt32, processName: StringPtr!, processNumber: ProcessSerialNumber, processType: UInt32, processSignature: OSType, processMode: UInt32, processLocation: Ptr!, processSize: UInt32, processFreeMem: UInt32, processLauncher: ProcessSerialNumber, processLaunchDate: UInt32, processActiveTime: UInt32, processAppRef: FSRefPtr!, processTempMemTotal: UInt32, processPurgeableTempMemTotal: UInt32)

### Instance Properties

var processActiveTime: UInt32

var processAppRef: FSRefPtr!

var processFreeMem: UInt32

var processInfoLength: UInt32

var processLaunchDate: UInt32

var processLauncher: ProcessSerialNumber

var processLocation: Ptr!

var processMode: UInt32

var processName: StringPtr!

var processNumber: ProcessSerialNumber

var processPurgeableTempMemTotal: UInt32

var processSignature: OSType

var processSize: UInt32

var processTempMemTotal: UInt32

var processType: UInt32

