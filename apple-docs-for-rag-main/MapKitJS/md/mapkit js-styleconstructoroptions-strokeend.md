

- MapKit JS
- StyleConstructorOptions
-  strokeEnd 

Instance Property

# strokeEnd

The unit distance along the line where a stroke ends.

MapKit JS 5.45+

``` source
attribute number strokeEnd;
```

## Discussion

The value of this property must be a number between `0` and `1`. A value of `0` represents the beginning of the polyline, and a value of `1,` the default, represents the end. MapKit JS interprets values between `0` and `1` linearly along the length of the polyline.

The stroke is only visible for the overlay when strokeStart is less than strokeEnd.

## See Also

### Setting stroke styles

strokeColor

The stroke color of a line.

strokeOpacity

The opacity of the stroke color.

strokeStart

The unit distance along the line where a stroke begins.

lineGradient

The gradient to apply along the line.

