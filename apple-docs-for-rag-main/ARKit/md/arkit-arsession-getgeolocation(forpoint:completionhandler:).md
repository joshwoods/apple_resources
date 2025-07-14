

- ARKit
- ARSession
-  getGeoLocation(forPoint:completionHandler:) 

Instance Method

# getGeoLocation(forPoint:completionHandler:)

Converts a position in the framework’s local coordinate system to latitude, longitude and altitude.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func getGeoLocation(
    forPoint position: simd_float3,
    completionHandler: @escaping (CLLocationCoordinate2D, CLLocationDistance, (any Error)?) -> Void
)
```

``` source
func geoLocation(forPoint position: simd_float3) async throws -> (CLLocationCoordinate2D, CLLocationDistance)
```

## Parameters 

`position`  

Position in local coordinates to convert.

`completionHandler`  

Code that control will execute when this function returns. The session runs this code on its delegate queue. The parameters are:

coordinate  
Location coordinates (latitude, longitude).

altitude  
The altitude.

error  
The reason, if conversion fails.

## Discussion

ARKit refers to its local coordinate space as “world” coordinate space, but this is different from geographic coordinates. For more information on ARKit’s coordinate space, see setWorldOrigin(relativeTransform:).

To succeed, this function requires an ARGeoTrackingConfiguration session with state equal to ARGeoTrackingStatus.State.localized.

