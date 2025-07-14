

- WebKit JS
- DeviceOrientationEvent
-  alpha 

Instance Property

# alpha

The rotation, in degrees, of the device frame around its z-axis.

Safari Mobile 4.2+

``` source
readonly attribute unrestricted double alpha;
```

## Discussion

Values are between 0 and 360. This property is `null` if the device cannot provide this angle.

## See Also

### Getting Orientation Event Properties

beta

The rotation, in degrees, of the device frame around its x-axis.

gamma

The rotation, in degrees, of the device frame around its y-axis.

