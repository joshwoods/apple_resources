

- ARKit
- ImageTrackingProvider
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the current runtime environment supports image-tracking providers.

visionOS 1.0+

``` source
static var isSupported: Bool { get }
```

## See Also

### Creating an image-tracking provider

init(referenceImages: [ReferenceImage])

Creates an image-tracking provider that tracks the reference images you supply.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for tracking images.

