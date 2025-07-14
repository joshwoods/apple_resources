

- ARKit
- CameraFrameProvider
-  CameraFrameProvider.CameraFrameUpdates 

Structure

# CameraFrameProvider.CameraFrameUpdates

A sequence of camera frames.

visionOS 2.0+

``` source
struct CameraFrameUpdates
```

## Topics

### Instance properties

static var isSupported: Bool

A Boolean value that indicates whether this device supports the camera frame provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The authorization types you need to use the camera frame provider.

### Instance methods

func makeAsyncIterator() -> CameraFrameProvider.CameraFrameUpdates.Iterator

### Iterating over camera updates

struct Iterator

An asynchronous iterator that produces camera frame elements on an asynchronous sequence.

### Type aliases

typealias Element

The type of element produced by this asynchronous sequence of camera frame structures.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Getting camera frame updates

func cameraFrameUpdates(for: CameraVideoFormat) -> CameraFrameProvider.CameraFrameUpdates?

Gets a sequence of camera frame updates for a given video format.

