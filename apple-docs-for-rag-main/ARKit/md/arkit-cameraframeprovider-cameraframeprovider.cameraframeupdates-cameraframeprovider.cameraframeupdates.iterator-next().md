

- ARKit
- CameraFrameProvider
- CameraFrameProvider.CameraFrameUpdates
- CameraFrameProvider.CameraFrameUpdates.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there’s no next element.

visionOS 2.0+

``` source
mutating func next() async -> CameraFrameProvider.CameraFrameUpdates.Element?
```

## Return Value

The next element, if it exists, or nil to signal the end of the sequence.

