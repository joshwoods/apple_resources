

- RoomPlan
- RoomCaptureSession
-  RoomCaptureSession.CaptureError 

Enumeration

# RoomCaptureSession.CaptureError

Errors that can occur during a room-capture session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
enum CaptureError
```

## Overview

The `error` argument of a room-capture session delgate’s captureSession(_:didEndWith:error:) function is of this type.

## Topics

### Identifying the error cause

case deviceNotSupported

An error that indicates that the framework doesn’t support the user’s device.

case deviceTooHot

An error that indicates when the device thermal metrics surpass the framework’s limitations.

case exceedSceneSizeLimit

An error that indicates when the scene size grows past the framework’s limitations.

case invalidARConfiguration

An error that indicates when the ARKit session runs an unsupported configuration.

case worldTrackingFailure

An error that indicates an issue with the underlying ARKit session.

case internalError

An error that indicates when the framework encounters an unexpected error case.

### Inspecting error information

var errorDescription: String?

A human-readable explanation for the error.

var failureReason: String?

A localized message describing the reason for the failure.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var localizedDescription: String

Retrieve the localized description for this error.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

### Comparing errors

static func == (RoomCaptureSession.CaptureError, RoomCaptureSession.CaptureError) -> Bool

Determines whether two errors are equal.

static func != (Self, Self) -> Bool

Determines whether two errors aren’t equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

## See Also

### Responding to events

var delegate: (any RoomCaptureSessionDelegate)?

An object that observes important events in the room-scanning process.

