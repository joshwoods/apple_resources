

- MapKit JS
- GeoJSONDelegate
-  geoJSONDidComplete 

Instance Method

# geoJSONDidComplete

Completes the GeoJSON import.

MapKit JS 5.0+

``` source
void geoJSONDidComplete(
 ItemCollection result,
 Object geoJSON
);
```

## Parameters 

`result`  

The mapped item collection.

`geoJSON`  

The original parsed GeoJSON object.

## Discussion

After MapKit JS loads the GeoJSON data and converts it to MapKit objects, the framework calls geoJSONDidComplete with the resulting ItemCollection, which reflects any provided customizations. This is the same value that returns directly from importGeoJSON in the synchronous case.

## See Also

### Handling errors and completion

geoJSONDidError

Indicates when the GeoJSON import fails.

