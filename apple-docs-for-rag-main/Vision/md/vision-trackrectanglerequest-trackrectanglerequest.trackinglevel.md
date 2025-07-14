

- Vision
- TrackRectangleRequest
-  TrackRectangleRequest.TrackingLevel 

Enumeration

# TrackRectangleRequest.TrackingLevel

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum TrackingLevel
```

## Topics

### Getting the tracking levels

case accurate

case fast

## Relationships

### Conforms To

- CaseIterable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a request

let inputObservation: any QuadrilateralProviding &amp; VisionObservation

The object to track.

protocol QuadrilateralProviding

A protocol for objects that have a bounding quadrilateral.

var trackingLevel: TrackRectangleRequest.TrackingLevel

The tracking quality preference.

