

- Core Media I/O
-  CMIODeviceAVCCommand 

Structure

# CMIODeviceAVCCommand

Mac Catalyst 13.1+macOS 10.7+

``` source
struct CMIODeviceAVCCommand
```

## Topics

### Initializers

init()

init(mCommand: UnsafeMutablePointer&lt;UInt8>!, mCommandLength: UInt32, mResponse: UnsafeMutablePointer&lt;UInt8>!, mResponseLength: UInt32, mResponseUsed: UInt32)

### Instance Properties

var mCommand: UnsafeMutablePointer&lt;UInt8>!

var mCommandLength: UInt32

var mResponse: UnsafeMutablePointer&lt;UInt8>!

var mResponseLength: UInt32

var mResponseUsed: UInt32

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct CMIODeviceRS422Command

struct CMIODeviceSMPTETimeCallback

struct CMIODeviceStreamConfiguration

struct CMIOObjectPropertyAddress

struct CMIOStreamDeck

struct CMIOStreamScheduledOutputNotificationProcAndRefCon

