

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.requestProgress(\_:fractionComplete:) 

Case

# PhotogrammetrySession.Output.requestProgress(\_:fractionComplete:)

A progress update provided by the session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case requestProgress(
    PhotogrammetrySession.Request,
    fractionComplete: Double
)
```

## Parameters 

`Request`  

The request in progress.

`fractionComplete`  

A number from `0.0` to `1.0` indicating the current progress for the request.

## See Also

### Monitoring request status

case requestComplete(PhotogrammetrySession.Request, PhotogrammetrySession.Result)

The session finished handling all pending requests.

case requestError(PhotogrammetrySession.Request, any Error)

The session aborted a request due to an error.

