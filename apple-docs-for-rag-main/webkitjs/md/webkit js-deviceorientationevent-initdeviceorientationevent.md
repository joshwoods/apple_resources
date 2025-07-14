

- WebKit JS
- DeviceOrientationEvent
-  initDeviceOrientationEvent 

Instance Method

# initDeviceOrientationEvent

Initializes a new device orientation event.

Safari Mobile 4.2+

``` source
void initDeviceOrientationEvent(
    optional DOMString type, 
    optional boolean bubbles, 
    optional boolean cancelable, 
    optional unrestricted double alpha, 
    optional unrestricted double beta, 
    optional unrestricted double gamma, 
    optional boolean absolute
);
```

## Parameters 

`type`  

The type of event. Pass `deviceorientation`.

`bubbles`  

A Boolean value that indicates whether this event is a bubbling event.

`cancelable`  

A Boolean value that indicates whether this event can be canceled.

`alpha`  

The rotation, in degrees, of the device frame around its z-axis.

`beta`  

The rotation, in degrees, of the device frame around its x-axis.

`gamma`  

The rotation, in degrees, of the device frame around its y-axis.

`compassHeading`  

A direction that is measured in degrees relative to magnetic north.

`compassAccuracy`  

The accuracy of the compass data in degrees.

## See Also

### Related Documentation

Safari Web Content Guide

