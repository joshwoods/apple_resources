

- RealityKit
- EntityTranslationGestureRecognizer
-  location(in:) 

Instance Method

# location(in:)

Returns the unprojected location of the gesture represented by the receiver in the space of the given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
func location(in entity: Entity?) -> SIMD3?
```

## Parameters 

`entity`  

An entity in whose space the location is computed. A `nil` entity will result in world space.

## Return Value

The 3D position identifying the location of the gesture in the space specified.

## Discussion

The location is typically the result of a centroid of touches for a gesture, unprojected onto the associated `entity`, and then converted into the space of the entity passed in, or world space if `nil` is passed in.

