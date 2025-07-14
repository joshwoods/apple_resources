

- ARKit
-  ar_mesh_anchors_get_count 

Function

# ar_mesh_anchors_get_count

Gets the number of mesh anchors in the collection.

visionOS 1.0+

``` source
extern size_t ar_mesh_anchors_get_count(ar_mesh_anchors_t mesh_anchors);
```

## See Also

### Scene reconstruction

ar_scene_reconstruction_configuration_t

ar_scene_reconstruction_mode_t

The additional kinds of information you can request about a person’s surroundings.

ar_scene_reconstruction_provider_create

Creates a provider that reconstructs the person’s surroundings.

ar_scene_reconstruction_provider_is_supported

Returns a Boolean value that indicates whether the current runtime environment supports scene reconstruction providers.

ar_scene_reconstruction_provider_get_required_authorization_type

Gets the types of authorizations needed to run scene reconstruction.

ar_scene_reconstruction_configuration_create

Creates a scene reconstruction configuration.

ar_scene_reconstruction_configuration_get_scene_reconstruction_mode

Gets the scene reconstruction mode.

ar_scene_reconstruction_configuration_set_scene_reconstruction_mode

Sets the scene reconstruction mode.

ar_scene_reconstruction_provider_set_update_handler

Sets the handler for receiving scene reconstruction updates.

ar_scene_reconstruction_provider_set_update_handler_f

Sets the handler for receiving scene reconstruction updates.

ar_mesh_classification_t

The kinds of classification a mesh anchor can have.

ar_mesh_anchor_get_geometry

Gets the shape of a mesh anchor.

ar_mesh_anchors_enumerate_anchors

Enumerates a collection of mesh anchors.

ar_mesh_anchors_enumerate_anchors_f

Enumerates a collection of mesh anchors.

ar_mesh_geometry_get_classification

Gets the classification of each face in the mesh.

