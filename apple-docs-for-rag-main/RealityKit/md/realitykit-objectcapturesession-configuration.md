

- RealityKit
- ObjectCaptureSession
-  configuration 

Instance Property

# configuration

The read-only `Configuration` used to start the capture session. The configuration can be set by passing it to the `start()` call and it remains immutable after the session is started successfully.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var configuration: ObjectCaptureSession.Configuration { get }
```

