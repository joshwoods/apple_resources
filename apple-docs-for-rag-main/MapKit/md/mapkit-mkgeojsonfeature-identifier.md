

- MapKit
- MKGeoJSONFeature
-  identifier 

Instance Property

# identifier

An optional identifier the class returns as a string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var identifier: String? { get }
```

## Discussion

Note that the GeoJSON specification states that the identifier can be a number or a string. However, this identifier returns as a string.

## See Also

### Feature properties

var geometry: [any MKShape &amp; MKGeoJSONObject]

The shape or shapes associated with the GeoJSON feature.

var properties: Data?

Optional serialized JSON data that corresponds to the properties key.

