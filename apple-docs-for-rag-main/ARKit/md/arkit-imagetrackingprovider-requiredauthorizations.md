

- ARKit
- ImageTrackingProvider
-  requiredAuthorizations 

Type Property

# requiredAuthorizations

The types of authorizations necessary for tracking images.

visionOS 1.0+

``` source
static var requiredAuthorizations: [ARKitSession.AuthorizationType] { get }
```

## See Also

### Creating an image-tracking provider

init(referenceImages: [ReferenceImage])

Creates an image-tracking provider that tracks the reference images you supply.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports image-tracking providers.

