

- Core Graphics
- CGLineCap
-  CGLineCap.square 

Case

# CGLineCap.square

A line with a squared-off end. Core Graphics extends the line beyond the endpoint of the path for a distance equal to half the line width.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case square
```

## See Also

### Constants

case butt

A line with a squared-off end. Core Graphics draws the line to extend only to the exact endpoint of the path. This is the default.

case round

A line with a rounded end. Core Graphics draws the line to extend beyond the endpoint of the path. The line ends with a semicircular arc with a radius of 1/2 the line’s width, centered on the endpoint.

