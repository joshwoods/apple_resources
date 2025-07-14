

- ARKit
-  ar_plane_anchor_get_alignment 

Function

# ar_plane_anchor_get_alignment

Gets the alignment — horizontal or vertical — of a plane anchor relative to gravity.

visionOS 1.0+

``` source
extern ar_plane_alignment_t ar_plane_anchor_get_alignment(ar_plane_anchor_t plane_anchor);
```

## See Also

### Plane detection

ar_plane_alignment_t

The kinds of alignment — horizontal or vertical — that a plane anchor can have.

ar_plane_classification_t

The kinds of object classification a plane anchor can have.

ar_plane_classification_ceiling

A ceiling.

ar_plane_classification_door

A door.

ar_plane_classification_floor

A floor.

ar_plane_classification_seat

A seat.

ar_plane_classification_status_not_available

A plane classification is currently unavailable.

ar_plane_classification_status_undetermined

A plane classification is undetermined.

ar_plane_classification_status_unknown

A plane classification isn’t one of the known classes.

ar_plane_classification_table

A table.

ar_plane_classification_wall

A wall.

ar_plane_classification_window

A window.

ar_plane_anchor_get_geometry

Gets the shape of a plane anchor.

ar_plane_anchor_get_plane_classification

Gets the kind of real-world object that ARKit determines the plane anchor might be.

ar_plane_anchors_enumerate_anchors

Enumerates a collection of plane anchors using the collection of plane anchors and the enumeratin handler you provide.

