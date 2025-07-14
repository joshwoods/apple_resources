

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Updates
- ObjectCaptureSession.Updates.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
mutating func next() async -> Element?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

