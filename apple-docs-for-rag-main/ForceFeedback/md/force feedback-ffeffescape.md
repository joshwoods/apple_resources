

- Force Feedback
-  FFEFFESCAPE 

Structure

# FFEFFESCAPE

The FFEFFESCAPE structure passes hardware-specific data directly to the Force Feedback plugIn.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct FFEFFESCAPE
```

## Topics

### Initializers

init()

init(dwSize: DWORD, dwCommand: DWORD, lpvInBuffer: UnsafeMutableRawPointer!, cbInBuffer: DWORD, lpvOutBuffer: UnsafeMutableRawPointer!, cbOutBuffer: DWORD)

### Instance Properties

var cbInBuffer: DWORD

Specifies the size, in bytes, of the **lpvInBuffer** buffer.

var cbOutBuffer: DWORD

On entry, specifies the size, in bytes, of the **lpvOutBuffer** buffer. On exit, specifies the number of bytes actually produced by the command.

var dwCommand: DWORD

Specifies a plugIn specific command number. Contact the hardware vendor for a list of valid commands and their parameters.

var dwSize: DWORD

Size, in bytes, of this structure. This member must be initialized before the structure is used.

var lpvInBuffer: UnsafeMutableRawPointer!

Buffer containing the data required to perform the operation.

var lpvOutBuffer: UnsafeMutableRawPointer!

Buffer in which the operation’s output data is returned.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct FFCAPABILITIES

Used by the FFDeviceGetForceFeedbackCapabilities method to retrieve device force-feedback capabilities.

struct FFCONDITION

A structure containing type-specific information for certain effects.

struct FFCONSTANTFORCE

Contains type-specific information for the CONSTANTFORCE effect.

struct FFCUSTOMFORCE

Contains type-specific information for the CUSTOMFORCE effect.

struct FFEFFECT

UsUsed by the FFDeviceCreateEffect method to initialize a new effect object. It is also used by the FFEffectSetParameters and FFEffectGetParameters functions.

struct FFENVELOPE

Used by the FFEFFECT structure to specify the optional envelope parameters for an effect.

struct FFPERIODIC

A structure containing type-specific information for certain effects.

struct FFRAMPFORCE

Contains type-specific information for the RAMPFORCE effect.

