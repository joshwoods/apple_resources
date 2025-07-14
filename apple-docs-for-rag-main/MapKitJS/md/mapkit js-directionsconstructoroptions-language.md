

- MapKit JS
- DirectionsConstructorOptions
-  language 

Instance Property

# language

A language ID that determines the language for route information.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

When you set language to a language, ID such as `fr-CA` or `en-GB`, MapKit JS returns step-by-step directions in the specified language, if available. If you don’t set language when initializing a mapkit.Directions object, the directions default to the language ID the system provides when initializing the map with init. If the map doesn’t have a specified language upon initialization, MapKit JS returns directions in the browser’s language setting.

For more information about language IDs, see Internationalization and Localization Guide.

