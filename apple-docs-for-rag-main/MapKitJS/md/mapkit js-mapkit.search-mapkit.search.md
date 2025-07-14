

- MapKit JS
- mapkit.Search
-  mapkit.Search 

Initializer

# mapkit.Search

Creates a search object with optional initial values that you provide.

MapKit JS 5.0+

``` source
new mapkit.Search(
 optional SearchConstructorOptions options
);
```

## Mentioned in 

MapKit JS 5

## Discussion

To use search, create an instance of a mapkit.Search. You can optionally set properties of the search object by providing a dictionary of SearchConstructorOptions on initialization.

```
var search = new mapkit.Search({
    language: "en-GB",
    getsUserLocation: true,
    region: map.region
});
```

## See Also

### Creating a search

SearchConstructorOptions

Options you provide when you create a search object.

