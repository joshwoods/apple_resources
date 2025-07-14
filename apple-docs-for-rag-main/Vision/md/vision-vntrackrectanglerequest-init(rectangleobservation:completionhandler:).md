

- Vision
- VNTrackRectangleRequest
-  init(rectangleObservation:completionHandler:) 

Initializer

# init(rectangleObservation:completionHandler:)

Creates a new rectangle tracking request with a rectangle observation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    rectangleObservation observation: VNRectangleObservation,
    completionHandler: VNRequestCompletionHandler? = nil
)
```

## Parameters 

`observation`  

A rectangle observation with bounding box and corner location information.

`completionHandler`  

The block to invoke after performing the request.

## See Also

### Initializing a Rectangle Tracking Request

convenience init(rectangleObservation: VNRectangleObservation)

Creates a new rectangle tracking request with a rectangle observation.

