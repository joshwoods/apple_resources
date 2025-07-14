

- ARKit
- ObjectTrackingProvider
-  requiredAuthorizations 

Type Property

# requiredAuthorizations

An array of authorization types the object-tracking provider requires.

visionOS 2.0+

``` source
static var requiredAuthorizations: [ARKitSession.AuthorizationType] { get }
```

## See Also

### Checking availability

static var isSupported: Bool

A Boolean value that indicates whether a device supports the object-tracking provider.

