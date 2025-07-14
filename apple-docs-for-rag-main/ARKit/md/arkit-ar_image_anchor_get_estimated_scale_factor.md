

- ARKit
-  ar_image_anchor_get_estimated_scale_factor 

Function

# ar_image_anchor_get_estimated_scale_factor

Gets the estimated scale factor between the tracked image’s physical size and the reference image’s size.

visionOS 1.0+

``` source
extern float ar_image_anchor_get_estimated_scale_factor(ar_image_anchor_t image_anchor);
```

## See Also

### Image tracking

ar_image_anchor_get_reference_image

Gets the reference image that this image anchor tracks.

ar_image_anchors_enumerate_anchors

Enumerates a collection of image anchors.

ar_image_anchors_enumerate_anchors_f

Enumerates a collection of image anchors.

ar_image_anchors_get_count

Gets the number of image anchors in the collection.

ar_image_tracking_provider_create

Creates an image tracking provider that tracks the reference images you supply.

ar_image_tracking_provider_is_supported

Returns a Boolean value that indicates whether the current runtime environment supports image tracking providers.

ar_image_tracking_provider_get_required_authorization_type

Gets the types of authorizations required to track images.

ar_image_tracking_provider_set_update_handler

Sets the handler for receiving image tracking updates.

ar_image_tracking_provider_set_update_handler_f

Sets the handler for receiving image tracking updates.

ar_image_tracking_configuration_add_reference_images

Adds reference images to the set to be tracked.

ar_image_tracking_configuration_create

Creates an image tracking configuration.

ar_image_tracking_configuration_t

ar_reference_images_t

A collection of reference images.

ar_reference_images_enumerator_t

A handler for enumerating a collection of reference images.

ar_reference_images_add_image

Adds a reference image to a collection.

