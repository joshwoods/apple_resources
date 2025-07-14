

- Vision
- VNTrackOpticalFlowRequest
-  init(completionHandler:) 

Initializer

# init(completionHandler:)

Creates a new request that tracks the optical from one image to another, with a system callback on completion.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(completionHandler: VNRequestCompletionHandler? = nil)
```

## Parameters 

`completionHandler`  

The callback the system invokes when it completes the request.

## See Also

### Creating an Optical Flow

init()

Creates a new request that tracks the optical from one image to another.

