

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.requestComplete(\_:\_:) 

Case

# PhotogrammetrySession.Output.requestComplete(\_:\_:)

The session finished handling all pending requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case requestComplete(PhotogrammetrySession.Request, PhotogrammetrySession.Result)
```

## See Also

### Monitoring request status

case requestProgress(PhotogrammetrySession.Request, fractionComplete: Double)

A progress update provided by the session.

case requestError(PhotogrammetrySession.Request, any Error)

The session aborted a request due to an error.

