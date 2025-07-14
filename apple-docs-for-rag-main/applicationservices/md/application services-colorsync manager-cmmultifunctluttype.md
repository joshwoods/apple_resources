

- Application Services
- ColorSync Manager
-  CMMultiFunctLutType 

Structure

# CMMultiFunctLutType

macOS 10.6+

``` source
struct CMMultiFunctLutType
```

## Topics

### Initializers

init()

init(typeDescriptor: OSType, reserved: UInt32, inputChannels: UInt8, outputChannels: UInt8, reserved2: UInt16, offsetBcurves: UInt32, offsetMatrix: UInt32, offsetMcurves: UInt32, offsetCLUT: UInt32, offsetAcurves: UInt32, data: UInt8)

### Instance Properties

var data: UInt8

var inputChannels: UInt8

var offsetAcurves: UInt32

var offsetBcurves: UInt32

var offsetCLUT: UInt32

var offsetMatrix: UInt32

var offsetMcurves: UInt32

var outputChannels: UInt8

var reserved: UInt32

var reserved2: UInt16

var typeDescriptor: OSType

