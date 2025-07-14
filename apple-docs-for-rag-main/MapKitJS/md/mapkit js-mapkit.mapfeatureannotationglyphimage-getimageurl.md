

- MapKit JS
- mapkit.MapFeatureAnnotationGlyphImage
-  getImageUrl 

Instance Method

# getImageUrl

Returns the image URL of the map feature.

MapKit JS 5.74+

``` source
void getImageUrl(
 number scale,
 function callback
);
```

## Discussion

The method returns the URL as the first argument of `callback`. The URL is a `blob:` URL. To avoid a memory leak, you need to revoke it with revokeObjectURL when you no longer need it.

