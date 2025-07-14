

- ARKit
- CameraFrameProvider
- CameraFrameProvider.CameraFrameUpdates
-  CameraFrameProvider.CameraFrameUpdates.Iterator 

Structure

# CameraFrameProvider.CameraFrameUpdates.Iterator

An asynchronous iterator that produces camera frame elements on an asynchronous sequence.

visionOS 2.0+

``` source
struct Iterator
```

## Topics

### Type methods

func next() async -> CameraFrameProvider.CameraFrameUpdates.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there’s no next element.

### Type aliases

typealias Element

The type of element produced by this asynchronous sequence of camera frame structures.

## Relationships

### Conforms To

- AsyncIteratorProtocol

