

- ARKit
-  CameraFrameProvider 

Class

# CameraFrameProvider

An object that provides camera streams.

visionOS 2.0+

``` source
final class CameraFrameProvider
```

## Overview

You use `CameraFrameProvider` to receive camera images for selected video formats.

## Topics

### Creating a camera frame provider

init()

Creates a camera frame provider.

### Getting information about the camera frame provider

var description: String

A textual representation of this camera frame provider.

var state: DataProviderState

The state of a camera frame provider.

### Getting camera frame updates

func cameraFrameUpdates(for: CameraVideoFormat) -> CameraFrameProvider.CameraFrameUpdates?

Gets a sequence of camera frame updates for a given video format.

struct CameraFrameUpdates

A sequence of camera frames.

### Enumerations

enum CameraPosition

Values that describe possible camera positions.

enum CameraType

Values that describe possible camera types.

### Type Properties

static var isSupported: Bool

A Boolean value that indicates whether this device supports the camera frame provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The authorization types you need to use the camera frame provider.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Camera sampling

struct CameraFrame

The representation of a camera frame.

struct CameraVideoFormat

A structure that represents a camera video format.

