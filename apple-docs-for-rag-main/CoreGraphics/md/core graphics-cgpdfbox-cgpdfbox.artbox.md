

- Core Graphics
- CGPDFBox
-  CGPDFBox.artBox 

Case

# CGPDFBox.artBox

The page art box—a rectangle, expressed in default user space units, defining the extent of the page’s meaningful content (including potential white space) as intended by the page’s creator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case artBox
```

## See Also

### Constants

case mediaBox

The page media box—a rectangle, expressed in default user space units, that defines the boundaries of the physical medium on which the page is intended to be displayed or printed

case cropBox

The page crop box—a rectangle, expressed in default user space units, that defines the visible region of default user space. When the page is displayed or printed, its contents are to be clipped to this rectangle.

case bleedBox

The page bleed box—a rectangle, expressed in default user space units, that defines the region to which the contents of the page should be clipped when output in a production environment.

case trimBox

The page trim box—a rectangle, expressed in default user space units, that defines the intended dimensions of the finished page after trimming.

