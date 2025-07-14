

- MapKit JS
- MapKitInitOptions
-  libraries 

Instance Property

# libraries

An array of libraries to load at initialization.

MapKit JS 5.73+

``` source
attribute string[] libraries;
```

## Discussion

Note

The full bundle of MapKit JS ignores this option.

MapKit JS divides its interfaces into libraries that you can specify when loading the framework. To optimize your app load time, pick only the interfaces you need:

- `services` — All services interfaces (such as Search and Geocoder) and relevant data types.

- `full-map` — All `mapkit.Map` features and relevant data types.

- `map` — Basic `mapkit.Map` features without overlays, annotations, and relevant data types.

- `overlays` — Overlays, data types, and displays on `mapkit.Map`.

- `annotations` — Annotations, data types, and displays on `mapkit.Map`.

- `geojson` — The GeoJSON importer.

- `user-location` — User location display and controls on `mapkit.Map`.

You can set the libraries to load statically by defining them within script tag in the `data-libraries` attribute or in the load method, or by passing a `libraries` property in the init options.

