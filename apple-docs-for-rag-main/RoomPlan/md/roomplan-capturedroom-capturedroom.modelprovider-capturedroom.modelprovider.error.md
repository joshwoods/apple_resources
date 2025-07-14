

- RoomPlan
- CapturedRoom
- CapturedRoom.ModelProvider
-  CapturedRoom.ModelProvider.Error 

Enumeration

# CapturedRoom.ModelProvider.Error

Errors that can occur when managing 3D model association with categories and attributes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum Error
```

## Overview

The `modelFileURL` functions can throw an error of this type, such as `CapturedRoom/ModelProvider/modelFileURL(for:)-42iz3`.

## Topics

### Interpreting the error

case attributeCombinationNotSupported

An error that indicates the framework doesn’t support the attributes set in a model-URL query.

case nonExistingFile(url: URL)

An error that indicates a model-URL query failed to return a result.

### Inspecting error information

var errorDescription: String?

A human-readable explanation for the particular model-provider error.

### Default Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Error
- LocalizedError
- Sendable

