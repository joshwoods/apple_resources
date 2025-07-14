

- ARKit
-  ar_world_tracking_add_anchor_completion_handler_t 

Type Alias

# ar_world_tracking_add_anchor_completion_handler_t

A handler to call upon completion of a request to add a world anchor.

visionOS 1.0+

``` source
typedef void (^)(NSObject *, _Bool, NSObject *) ar_world_tracking_add_anchor_completion_handler_t;
```

## See Also

### World tracking

ar_world_anchor_create_with_origin_from_anchor_transform

Creates a world anchor from a position and orientation in world space.

ar_world_tracking_remove_anchor_completion_handler_t

A handler to call upon completion of a request to remove a world anchor.

ar_world_tracking_anchor_update_handler_t

A handler for receiving updates to world anchors.

ar_world_tracking_configuration_create

Creates a world tracking configuration.

ar_world_anchors_enumerate_anchors

Enumerates a collection of world anchors.

ar_world_anchors_enumerate_anchors_f

Enumerates a collection of world anchors.

ar_world_anchors_get_count

Gets the number of world anchors in the collection.

ar_world_tracking_provider_create

Creates a world tracking provider.

ar_world_tracking_provider_is_supported

Returns a Boolean value that indicates whether the current runtime environment supports world tracking providers.

ar_world_tracking_provider_query_device_anchor_at_timestamp

Queries the predicted pose of the current device at a given time.

ar_world_tracking_provider_add_anchor

Adds a world anchor you supply to the set of currently tracked anchors.

ar_world_tracking_provider_add_anchor_f

Adds a world anchor you supply to the set of currently tracked anchors.

ar_world_tracking_provider_get_required_authorization_type

Gets the types of authorizations required to track world anchors.

ar_world_tracking_provider_set_anchor_update_handler

Sets the handler for receiving world tracking updates.

ar_world_tracking_provider_set_anchor_update_handler_f

Sets the handler for receiving world tracking updates.

