

- Vision
- ClassificationObservation
-  hasPrecisionRecallCurve 

Instance Property

# hasPrecisionRecallCurve

A Boolean value that indicates whether the observation contains precision and recall curves.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var hasPrecisionRecallCurve: Bool { get }
```

## Discussion

If this property is `true`, then you can call precision and recall-related methods in this observation.

If this property is `false`, then the precision and recall-related methods don’t return meaningful data.

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let identifier: String

The classification label that identifies the type of observation.

