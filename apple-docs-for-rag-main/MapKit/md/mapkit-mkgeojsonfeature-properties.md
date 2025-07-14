

- MapKit
- MKGeoJSONFeature
-  properties 

Instance Property

# properties

Optional serialized JSON data that corresponds to the properties key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var properties: Data? { get }
```

## Discussion

MapKit exposes these optional properties but treats them as opaque.

## See Also

### Feature properties

var geometry: [any MKShape &amp; MKGeoJSONObject]

The shape or shapes associated with the GeoJSON feature.

var identifier: String?

An optional identifier the class returns as a string.

