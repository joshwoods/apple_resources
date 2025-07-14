

- WebKit JS
- DeviceOrientationEvent
-  gamma 

Instance Property

# gamma

The rotation, in degrees, of the device frame around its y-axis.

Safari Mobile 4.2+

``` source
readonly attribute unrestricted double gamma;
```

## Discussion

Values are between -180 and 180. This property is `null` if the device cannot provide this angle.

## See Also

### Getting Orientation Event Properties

alpha

The rotation, in degrees, of the device frame around its z-axis.

beta

The rotation, in degrees, of the device frame around its x-axis.

