

- Application Services
- ApplicationServices Structures
- PixMap
-  cmpCount 

Instance Property

# cmpCount

The number of components used to represent a color for a pixel. With indexed pixels, each pixel is a single value representing an index in a color table, and therefore this field contains the value 1; the index is the single component. With direct pixels, each pixel contains three components (one integer each for the intensities of red, green, and blue) so this field contains the value 3.

macOS 10.0+

``` source
var cmpCount: Int16
```

