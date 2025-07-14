

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.requestError(\_:\_:) 

Case

# PhotogrammetrySession.Output.requestError(\_:\_:)

The session aborted a request due to an error.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case requestError(PhotogrammetrySession.Request, any Error)
```

## Parameters 

`Request`  

The request in progress.

`Error`  

Details of the error.

## See Also

### Monitoring request status

case requestProgress(PhotogrammetrySession.Request, fractionComplete: Double)

A progress update provided by the session.

case requestComplete(PhotogrammetrySession.Request, PhotogrammetrySession.Result)

The session finished handling all pending requests.

