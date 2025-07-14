

- HealthKit
- HKGlassesLensSpecification
-  prism 

Instance Property

# prism

An object that contains information about the eye alignment correction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var prism: HKVisionPrism? { get }
```

## See Also

### Accessing the specification’s data

var farPupillaryDistance: HKQuantity?

The distance between the pupil and the center of the nose when looking at an object far away, measured in mm.

var nearPupillaryDistance: HKQuantity?

The distance between the pupil and the center of the nose when looking at a nearby object, measured in mm.

var vertexDistance: HKQuantity?

The distance between the back of the lens and the eye, measured in mm.

