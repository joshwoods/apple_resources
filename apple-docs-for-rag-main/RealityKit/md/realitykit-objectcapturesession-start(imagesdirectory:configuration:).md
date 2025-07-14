

- RealityKit
- ObjectCaptureSession
-  start(imagesDirectory:configuration:) 

Instance Method

# start(imagesDirectory:configuration:)

Starts the session with the provided output image directory and optional checkpoint directory.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func start(
    imagesDirectory: URL,
    configuration: ObjectCaptureSession.Configuration = Configuration()
)
```

## Parameters 

`imagesDirectory`  

A directory to save the images.

`configuration`  

A configuration specifying session options.

## Discussion

The directory that `imagesDirectory` points to needs to be an empty and writable directory or it is an error. Likewise, if `checkpointDirectory` is provided, it needs to be empty if it already exists. If the directory does not exist, it is created for you. If it cannot be, the session moves to `.failed` state.

This call is only valid once on a newly created session.

