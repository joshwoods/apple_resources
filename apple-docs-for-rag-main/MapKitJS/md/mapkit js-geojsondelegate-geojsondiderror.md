

- MapKit JS
- GeoJSONDelegate
-  geoJSONDidError 

Instance Method

# geoJSONDidError

Indicates when the GeoJSON import fails.

MapKit JS 5.0+

``` source
void geoJSONDidError(
 Error error,
 Object geoJSON
);
```

## Parameters 

`error`  

An `Error` instance related to the last blocking error.

`geoJSON`  

The original parsed GeoJSON object.

## Discussion

MapKit JS calls this method when the GeoJSON fails to load.

## See Also

### Handling errors and completion

geoJSONDidComplete

Completes the GeoJSON import.

