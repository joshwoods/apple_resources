

- Core Graphics
- CGLineJoin
-  CGLineJoin.miter 

Case

# CGLineJoin.miter

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case miter
```

## Discussion

A join with a sharp (angled) corner. Core Graphics draws the outer sides of the lines beyond the endpoint of the path, until they meet. If the length of the miter divided by the line width is greater than the miter limit, a bevel join is used instead. This is the default. To set the miter limit, see setMiterLimit(_:).

## See Also

### Constants

case round

A join with a rounded end. Core Graphics draws the line to extend beyond the endpoint of the path. The line ends with a semicircular arc with a radius of 1/2 the line’s width, centered on the endpoint.

case bevel

A join with a squared-off end. Core Graphics draws the line to extend beyond the endpoint of the path, for a distance of 1/2 the line’s width.

