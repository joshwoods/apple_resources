

- Application Services
- ApplicationServices Structures
-  LaunchParamBlockRec 

Structure

# LaunchParamBlockRec

macOS 10.0+

``` source
struct LaunchParamBlockRec
```

## Topics

### Initializers

init()

init(reserved1: UInt32, reserved2: UInt16, launchBlockID: UInt16, launchEPBLength: UInt32, launchFileFlags: UInt16, launchControlFlags: LaunchFlags, launchAppRef: FSRefPtr!, launchProcessSN: ProcessSerialNumber, launchPreferredSize: UInt32, launchMinimumSize: UInt32, launchAvailableSize: UInt32, launchAppParameters: AppParametersPtr!)

### Instance Properties

var launchAppParameters: AppParametersPtr!

var launchAppRef: FSRefPtr!

var launchAvailableSize: UInt32

var launchBlockID: UInt16

var launchControlFlags: LaunchFlags

var launchEPBLength: UInt32

var launchFileFlags: UInt16

var launchMinimumSize: UInt32

var launchPreferredSize: UInt32

var launchProcessSN: ProcessSerialNumber

var reserved1: UInt32

var reserved2: UInt16

