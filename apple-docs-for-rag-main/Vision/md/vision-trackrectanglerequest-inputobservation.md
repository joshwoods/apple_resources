

- Vision
- TrackRectangleRequest
-  inputObservation 

Instance Property

# inputObservation

The object to track.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final let inputObservation: any QuadrilateralProviding & VisionObservation
```

## See Also

### Inspecting a request

protocol QuadrilateralProviding

A protocol for objects that have a bounding quadrilateral.

var trackingLevel: TrackRectangleRequest.TrackingLevel

The tracking quality preference.

enum TrackingLevel

