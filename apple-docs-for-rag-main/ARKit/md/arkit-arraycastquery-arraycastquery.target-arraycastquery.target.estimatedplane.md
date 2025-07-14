

- ARKit
- ARRaycastQuery
- ARRaycastQuery.Target
-  ARRaycastQuery.Target.estimatedPlane 

Case

# ARRaycastQuery.Target.estimatedPlane

A raycast target that specifies nonplanar surfaces, or planes about which ARKit can only estimate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
case estimatedPlane
```

## Discussion

A raycast with this target intersects feature points around the ray that ARKit estimates may be a real-world surface.

When combined with ARRaycastQuery.TargetAlignment.any, ARKit bases estimated plane alignment on the normal of the surface.

When you set your world-tracking configuration’s sceneReconstruction to one of the `mesh` options, ARKit allows a raycast with this target (and target-alignment ARRaycastQuery.TargetAlignment.any) to intersect the scene mesh. Then the raycast result can include points even on nonplanar surfaces or surfaces that have few or no features, such as a white wall. If you set sceneReconstruction to ARSceneReconstructionNone, raycasts ignore the scene mesh.

## See Also

### Targets

case existingPlaneGeometry

A raycast target that requires a plane to have a definitive size and shape.

case existingPlaneInfinite

A raycast target that specifies a detected plane, regardless of its size and shape.

