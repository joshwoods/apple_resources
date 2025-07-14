

- RoomPlan
- StructureBuilder
-  StructureBuilder.BuildError 

Enumeration

# StructureBuilder.BuildError

Errors that can occur capturedStructure merging processing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 16.0–1.0Deprecated

``` source
enum BuildError
```

## Overview

The structure builder (StructureBuilder) function capturedStructure(from:) can throw an error of this type.

## Topics

### Operators

static func == (StructureBuilder.BuildError, StructureBuilder.BuildError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case deviceNotSupported

An error that indicates that the framework doesn’t support the user’s device.

case exceedSceneSizeLimit

An error that indicates when the scene size grows past the framework’s limitations.

case insufficientInput

An error that indicates the framework expects more captured room data.

case internalError

An error that indicates when the framework encounters an unexpected error case.

case invalidInput

An error that indicates the framework encounters invalid captured room data.

case invalidRoomLocation

An error that indicates one or more rooms reside in a different vicinity.

### Instance Properties

var errorDescription: String?

A human-readable explanation of the error.

var hashValue: Int

The hash value.

### Instance Methods

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

