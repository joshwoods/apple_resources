

- ARKit
-  ar_device_anchor_get_tracking_state 

Function

# ar_device_anchor_get_tracking_state

Gets the tracking state of the device anchor.

visionOS 2.0+

``` source
extern ar_device_anchor_tracking_state_t ar_device_anchor_get_tracking_state(ar_device_anchor_t anchor);
```

## Parameters 

`anchor`  

The anchor.

## Return Value

The tracking state of this anchor.

## See Also

### Device anchor functions

ar_device_anchor_get_identifier

ar_device_anchor_get_origin_from_anchor_transform

ar_device_anchor_get_timestamp

ar_device_anchor_is_tracked

