

- Application Services
- ApplicationServices Structures
- LaunchParamBlockRec
-  init(reserved1:reserved2:launchBlockID:launchEPBLength:launchFileFlags:launchControlFlags:launchAppRef:launchProcessSN:launchPreferredSize:launchMinimumSize:launchAvailableSize:launchAppParameters:) 

Initializer

# init(reserved1:reserved2:launchBlockID:launchEPBLength:launchFileFlags:launchControlFlags:launchAppRef:launchProcessSN:launchPreferredSize:launchMinimumSize:launchAvailableSize:launchAppParameters:)

macOS 10.9+Xcode 9.0+

``` source
init(
    reserved1: UInt32,
    reserved2: UInt16,
    launchBlockID: UInt16,
    launchEPBLength: UInt32,
    launchFileFlags: UInt16,
    launchControlFlags: LaunchFlags,
    launchAppRef: FSRefPtr!,
    launchProcessSN: ProcessSerialNumber,
    launchPreferredSize: UInt32,
    launchMinimumSize: UInt32,
    launchAvailableSize: UInt32,
    launchAppParameters: AppParametersPtr!
)
```

