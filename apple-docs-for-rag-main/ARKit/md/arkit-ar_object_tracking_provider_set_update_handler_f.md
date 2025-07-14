

- ARKit
-  ar_object_tracking_provider_set_update_handler_f 

Function

# ar_object_tracking_provider_set_update_handler_f

visionOS 2.0+

``` source
extern void ar_object_tracking_provider_set_update_handler_f(ar_object_tracking_provider_t object_tracking_provider, dispatch_queue_t object_tracking_updates_queue, void * context, ar_object_tracking_update_handler_function_t object_tracking_update_handler_function);
```

## See Also

### Object tracking provider functions

ar_object_tracking_provider_copy_all_object_anchors

ar_object_tracking_provider_create

ar_object_tracking_provider_get_required_authorization_type

ar_object_tracking_provider_is_supported

ar_object_tracking_provider_set_update_handler

ar_object_tracking_error_code_t

An enumeration that describes object tracking errors.

object_tracking_h

