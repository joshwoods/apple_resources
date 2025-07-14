

- ARKit
- ImageTrackingProvider
-  init(referenceImages:) 

Initializer

# init(referenceImages:)

Creates an image-tracking provider that tracks the reference images you supply.

visionOS 1.0+

``` source
init(referenceImages: [ReferenceImage])
```

## Parameters 

`referenceImages`  

An array of known images to track in a person’s surroundings.

## See Also

### Creating an image-tracking provider

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports image-tracking providers.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for tracking images.

