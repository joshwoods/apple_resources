

- Core Graphics
- CGLineCap
-  CGLineCap.butt 

Case

# CGLineCap.butt

A line with a squared-off end. Core Graphics draws the line to extend only to the exact endpoint of the path. This is the default.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case butt
```

## See Also

### Constants

case round

A line with a rounded end. Core Graphics draws the line to extend beyond the endpoint of the path. The line ends with a semicircular arc with a radius of 1/2 the line’s width, centered on the endpoint.

case square

A line with a squared-off end. Core Graphics extends the line beyond the endpoint of the path for a distance equal to half the line width.

