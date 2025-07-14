

- Application Services
- ApplicationServices Structures
- ProcessInfoRec
-  init(processInfoLength:processName:processNumber:processType:processSignature:processMode:processLocation:processSize:processFreeMem:processLauncher:processLaunchDate:processActiveTime:processAppRef:) 

Initializer

# init(processInfoLength:processName:processNumber:processType:processSignature:processMode:processLocation:processSize:processFreeMem:processLauncher:processLaunchDate:processActiveTime:processAppRef:)

macOS 10.9+Xcode 9.0+

``` source
init(
    processInfoLength: UInt32,
    processName: StringPtr!,
    processNumber: ProcessSerialNumber,
    processType: UInt32,
    processSignature: OSType,
    processMode: UInt32,
    processLocation: Ptr!,
    processSize: UInt32,
    processFreeMem: UInt32,
    processLauncher: ProcessSerialNumber,
    processLaunchDate: UInt32,
    processActiveTime: UInt32,
    processAppRef: FSRefPtr!
)
```

