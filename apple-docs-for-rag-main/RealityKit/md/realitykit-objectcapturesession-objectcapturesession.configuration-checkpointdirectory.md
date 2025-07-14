

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Configuration
-  checkpointDirectory 

Instance Property

# checkpointDirectory

An optional directory to store data about session progress which may be used to speed up on-device reconstruction by passing into the `PhotogrammetrySession.Configuration`. If you provide a value for `checkpointDirectory`, it also needs to point to an empty, writable directory. If the directory is not writable or already contains data, the session moves to the `.failed(Error)` state.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
var checkpointDirectory: URL?
```

