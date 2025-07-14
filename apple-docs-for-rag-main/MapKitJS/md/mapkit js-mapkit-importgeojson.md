

- MapKit JS
- mapkit
-  importGeoJSON 

Instance Method

# importGeoJSON

Converts imported GeoJSON data to MapKit JS items.

MapKit JS 5.0+

``` source
ItemCollection|Error importGeoJSON(
 string|Object data,
 optional function|GeoJSONDelegate callback
);
```

## Parameters 

`data`  

The original GeoJSON data, either a URL to a GeoJSON file, or a GeoJSON object.

`callback`  

A callback function that MapKit JS requires if you provide a URL for the `data` parameter. It’s optional, otherwise.

## Return Value

If the data argument is a GeoJSON object instead of a URL and you don’t provide a `callback` function, importGeoJSON returns an ItemCollection. If the data import fails, this method returns an error.

## Mentioned in 

MapKit JS 5

## Discussion

This function converts imported GeoJSON data into MapKit JS items, which are annotations, overlays, and ItemCollection objects. Access the original GeoJSON data through the object’s data property.

You can customize the import by implementing a GeoJSONDelegate callback:

- If you provide a GeoJSON object for the `data` parameter, importGeoJSON returns the result directly. However, the system uses the optional callback, if you provide it.

- If you provide a URL to a GeoJSON file in the `data` parameter, you need to provide a callback function.

MapKit JS invokes this callback with two arguments, `error` on failure and `result` on success, as follows:

`error` (Error)  
Contains an error code and descriptive message.

`result` (Item)  
The resulting ItemCollection. MapKit JS stores the raw GeoJSON to use for generating the object in the object’s `data` property.

Note

GeoJSON is a format that encodes geographic data. See the GeoJSON standard specification RFC 7946 for more information.

## See Also

### Geographical features

GeoJSONDelegate

A delegate object that controls a GeoJSON import to override default behavior and provide custom style.

ItemCollection

A tree structure containing annotations, overlays, and nested item collection objects.

Displaying Indoor Maps with MapKit JS

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest in your browser.

