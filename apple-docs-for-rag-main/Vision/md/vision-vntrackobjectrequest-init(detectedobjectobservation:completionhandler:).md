

- Vision
- VNTrackObjectRequest
-  init(detectedObjectObservation:completionHandler:) 

Initializer

# init(detectedObjectObservation:completionHandler:)

Creates a new object tracking request with a detected object observation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    detectedObjectObservation observation: VNDetectedObjectObservation,
    completionHandler: VNRequestCompletionHandler? = nil
)
```

## Parameters 

`observation`  

A detected object observation with bounding box information.

`completionHandler`  

The callback to invoke after performing the request.

## See Also

### Initializing an Object Tracking Request

init(detectedObjectObservation: VNDetectedObjectObservation)

Creates a new object tracking request with a detected object observation.

