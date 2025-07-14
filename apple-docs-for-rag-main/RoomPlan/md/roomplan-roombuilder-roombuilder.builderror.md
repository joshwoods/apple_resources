

- RoomPlan
- RoomBuilder
-  RoomBuilder.BuildError 

Enumeration

# RoomBuilder.BuildError

Errors that can occur during captured room-data processing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
enum BuildError
```

## Overview

The room builder (RoomBuilder) function capturedRoom(from:) can throw an error of this type.

## Topics

### Interpreting the error cause

case insufficientInput

An error that indicates the framework expects more captured room data.

case invalidInput

An error that indicates the framework encounters invalid captured room data.

case exceedSceneSizeLimit

An error that indicates when the scene size grows past the framework’s limitations.

case internalError

An error that indicates when the framework encounters an unexpected error case.

case deviceNotSupported

An error that indicates that the framework doesn’t support the user’s device.

### Inspecting error information

var errorDescription: String?

A localized message describing what error occurred.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

var localizedDescription: String

Retrieve the localized description for this error.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var failureReason: String?

A localized message describing the reason for the failure.

### Comparing build errors

static func == (RoomBuilder.BuildError, RoomBuilder.BuildError) -> Bool

Determines whether two errors are equal.

static func != (Self, Self) -> Bool

Determines whether two errors aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

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

