

- LockedCameraCapture
- LockedCameraCaptureSession
-  LockedCameraCaptureSession.ApplicationLaunchError 

Enumeration

# LockedCameraCaptureSession.ApplicationLaunchError

Indicates why launching the extension’s containing app failed.

iOS 18.0+iPadOS 18.0+

``` source
enum ApplicationLaunchError
```

## Topics

### Operators

static func == (LockedCameraCaptureSession.ApplicationLaunchError, LockedCameraCaptureSession.ApplicationLaunchError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case applicationNotFound

An error that the launch failed because the system didn’t find the application.

case authenticationFailed

An error that the launch failed because authentication failed and the device is locked.

case unknown

An error that the launch failed with an unknown error.

### Instance Properties

var errorCode: Int

An integer value that represents the error code.

var failureReason: String?

A string that describes the error that occurred.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var errorDomain: String

The domain for errors that can occur when launching the extension’s containing app.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

