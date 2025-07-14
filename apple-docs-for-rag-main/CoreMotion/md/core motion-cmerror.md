

- Core Motion
-  CMError 

Structure

# CMError

Defines motion errors.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
struct CMError
```

## Topics

### Errors

var CMErrorDeviceRequiresMovement: CMError

The device must move for a sampling of motion data to occur.

var CMErrorInvalidAction: CMError

The specified action is invalid.

var CMErrorInvalidParameter: CMError

The specified parameter is invalid.

var CMErrorMotionActivityNotAuthorized: CMError

The app isn’t currently authorized to use motion activity support.

var CMErrorMotionActivityNotAvailable: CMError

Motion activity support isn’t available on the current device.

var CMErrorMotionActivityNotEntitled: CMError

The app is missing an entitlement for the requested activity.

var CMErrorNilData: CMError

Core Motion didn’t return any data.

var CMErrorNULL: CMError

No error occurred.

var CMErrorNotAuthorized: CMError

The app isn’t authorized to use the Core Motion framework.

var CMErrorNotAvailable: CMError

The requested service isn’t available on this device.

var CMErrorNotEntitled: CMError

The app is missing a required entitlement.

var CMErrorSize: CMError

The data is the incorrect size.

var CMErrorTrueNorthNotAvailable: CMError

True north isn’t available on this device.

var CMErrorUnknown: CMError

An unknown error occurred.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Understanding Errors

let CMErrorDomain: String

The error domain for Core Motion.

