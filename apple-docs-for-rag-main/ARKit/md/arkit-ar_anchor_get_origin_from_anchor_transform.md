

- ARKit
-  ar_anchor_get_origin_from_anchor_transform 

Function

# ar_anchor_get_origin_from_anchor_transform

Gets the transform from the anchor to the origin coordinate system.

visionOS 1.0+

``` source
extern simd_float4x4 ar_anchor_get_origin_from_anchor_transform(ar_anchor_t anchor);
```

## See Also

### Anchors

ar_anchor_get_identifier

Gets the unique identifier that distinguishes this anchor from all other anchors.

ar_anchor_get_timestamp

Gets the timestamp corresponding to the anchor.

ar_trackable_anchor_is_tracked

Returns a Boolean value that indicates whether ARKit is tracking an anchor.

ar_anchor_t

The identity, location, and orientation of an object in world space.

ar_mesh_anchor_t

A surface’s position in a person’s surroundings.

ar_mesh_anchors_t

A collection of mesh anchors.

ar_mesh_anchors_enumerator_t

A handler for enumerating a collection of mesh anchors.

ar_image_anchor_t

A 2D image’s position in a person’s surroundings.

ar_image_anchors_t

A collection of image anchors.

ar_image_anchors_enumerator_t

A handler for enumerating a collection of image anchors.

ar_hand_anchor_t

A hand’s position in a person’s surroundings.

ar_trackable_anchor_t

An anchor that can gain and lose its tracking state over the course of a session.

ar_world_anchor_t

A fixed location in a person’s surroundings.

ar_world_anchors_t

A collection of world anchors.

ar_world_anchors_enumerator_t

A handler for enumerating a collection of world anchors.

