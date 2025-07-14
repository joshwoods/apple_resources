

- RealityKit
- ObjectCaptureSession
-  ObjectCaptureSession.Configuration 

Structure

# ObjectCaptureSession.Configuration

The configuration options for the session which are passed into the `start(imagesDirectory:configuration:)` call.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
struct Configuration
```

## Topics

### Initializers

init()

### Instance Properties

var checkpointDirectory: URL?

An optional directory to store data about session progress which may be used to speed up on-device reconstruction by passing into the `PhotogrammetrySession.Configuration`. If you provide a value for `checkpointDirectory`, it also needs to point to an empty, writable directory. If the directory is not writable or already contains data, the session moves to the `.failed(Error)` state.

var isOverCaptureEnabled: Bool

Enables the session to continue capturing even after the number of captured images exceeds `maximumNumberOfInputImages`. This setting is meant for use when the images are intended to be transferred to macOS for model reconstruction.

