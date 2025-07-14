

- MapKit
- MKGeoJSONFeature
-  geometry 

Instance Property

# geometry

The shape or shapes associated with the GeoJSON feature.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var geometry: [any MKShape & MKGeoJSONObject] { get }
```

## See Also

### Feature properties

var identifier: String?

An optional identifier the class returns as a string.

var properties: Data?

Optional serialized JSON data that corresponds to the properties key.

