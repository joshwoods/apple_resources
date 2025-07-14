

- MapKit JS
-  ImageDelegate 

Class

# ImageDelegate

An object you use to specify image URLs.

MapKit JS 5.74+

``` source
interface ImageDelegate
```

## Overview

In addition to using a dictionary object that defines image URLs for mapkit.ImageAnnotation or mapkit.MarkerAnnotation, you can specify an image delegate that allows you to return a URL dynamically or asynchronously.

```
```

MapKit JS calls this method with a pixel ratio value that your function uses to construct a URL to an appropriately scaled image, and returns it as the first argument of the callback, as in the following example:

```
```

## Topics

### Returning an image URL

getImageUrl

Returns the URL to an image of the specified scale.

## Relationships

### Inherits From

- mapkit.MapFeatureAnnotationGlyphImage

## See Also

### Delegates

FetchDelegate

An object to pass to a map feature annotation to fetch place objects instead of a callback function.

