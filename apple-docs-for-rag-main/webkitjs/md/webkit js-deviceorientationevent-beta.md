

- WebKit JS
- DeviceOrientationEvent
-  beta 

Instance Property

# beta

The rotation, in degrees, of the device frame around its x-axis.

Safari Mobile 4.2+

``` source
readonly attribute unrestricted double beta;
```

## Discussion

Values are between -90 and 90. This property is `null` if the device cannot provide this angle.

## See Also

### Getting Orientation Event Properties

alpha

The rotation, in degrees, of the device frame around its z-axis.

gamma

The rotation, in degrees, of the device frame around its y-axis.

