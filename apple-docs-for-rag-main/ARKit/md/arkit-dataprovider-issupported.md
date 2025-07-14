

- ARKit
- DataProvider
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the current runtime environment supports a particular provider type.

visionOS 1.0+

``` source
static var isSupported: Bool { get }
```

**Required**

## Discussion

For example, data providers are not supported in Simulator.

## See Also

### Inspecting a data provider type

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The kinds of authorization you need to use a particular data provider type.

**Required**

