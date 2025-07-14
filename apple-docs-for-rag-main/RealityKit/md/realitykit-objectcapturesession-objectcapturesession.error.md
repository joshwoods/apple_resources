

- RealityKit
- ObjectCaptureSession
-  ObjectCaptureSession.Error 

Enumeration

# ObjectCaptureSession.Error

Errors associated with the top-level computation of this class.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
enum Error
```

## Topics

### Enumeration Cases

case cancelled

The user requested that the session be canceled and the session is now canceled. Another session may now be created.

case directoryNotEmpty(URL)

We cannot continue a pre-existing capture, so if an output directory is provided that already exists and it is not empty, this error is thrown.

case insufficientStorage(requiredBytes: Int64)

The session can’t be started since there is not enough storage space in the provided directories.

case sensorFailed

There was an ARKit failure in one of the sensors.

case trackingFailed

There was an unrecoverable error related to tracking the object or environment.

### Instance Properties

var localizedDescription: String

Retrieve the localized description for this error.

### Default Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Error
- LocalizedError
- Sendable

## See Also

### Monitoring the session

enum CaptureState

State of the capture session.

