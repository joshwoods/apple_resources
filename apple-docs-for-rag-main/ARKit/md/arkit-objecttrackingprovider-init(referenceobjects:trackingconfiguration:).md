

- ARKit
- ObjectTrackingProvider
-  init(referenceObjects:trackingConfiguration:) 

Initializer

# init(referenceObjects:trackingConfiguration:)

Creates an object-tracking provider.

visionOS 2.0+

``` source
init(
    referenceObjects: [ReferenceObject],
    trackingConfiguration: ObjectTrackingProvider.TrackingConfiguration? = nil
)
```

## Parameters 

`referenceObjects`  

The reference objects to look for

`trackingConfiguration`  

Optional parameters for configuring object tracking if not provided, the framework applies a set of default values.

## Discussion

The method clamps the numeric parameter values for configuring tracking if they’re outside their supported range.

