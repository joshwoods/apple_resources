

- RoomPlan
- CapturedRoom
-  CapturedRoom.Error 

Enumeration

# CapturedRoom.Error

Errors that can occur during a captured room export.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Error
```

## Overview

The captured room (CapturedRoom) function export(to:metadataURL:modelProvider:exportOptions:) can throw an error of this type.

## Topics

### Interpreting the error

case deviceNotSupported

An error that indicates that the framework doesn’t support the user’s device.

case urlInvalidFileExtension

An error that indicates that the URL contains an unsupported file extension.

case urlInvalidFilePath

An error that indicates that the URL references an invalid file path.

case urlInvalidScheme

An error that indicates that the URL prefix represents an unsupported scheme.

case urlMissingFileExtension

An error that indicates that the URL lacks a necessary file extension.

### Inspecting error information

var errorDescription: String?

A human-readable explanation of the error.

### Comparing errors

static func == (CapturedRoom.Error, CapturedRoom.Error) -> Bool

Determines whether two captured room errors are equal.

static func != (Self, Self) -> Bool

Determines whether two captured room errors aren’t equal.

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

