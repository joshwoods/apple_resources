

- MapKit
-  MKGeoJSONFeature 

Class

# MKGeoJSONFeature

The decoded representation of a GeoJSON feature.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKGeoJSONFeature
```

## Overview

A feature is an object with associated geometry and optional properties in JSON that you define. MapKit exposes these optional properties, but treats them as opaque. MKGeoJSONFeature is one of the classes that the GeoJSON decoder (MKGeoJSONDecoder) can return.

See the GeoJSON standards specification RFC 7946 for more information about `Feature` objects.

## Topics

### Feature properties

var geometry: [any MKShape &amp; MKGeoJSONObject]

The shape or shapes associated with the GeoJSON feature.

var identifier: String?

An optional identifier the class returns as a string.

var properties: Data?

Optional serialized JSON data that corresponds to the properties key.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKGeoJSONObject
- NSObjectProtocol

## See Also

### Geographical features

Displaying an Indoor Map

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest.

class MKGeoJSONDecoder

An object that decodes GeoJSON objects into MapKit types.

protocol MKGeoJSONObject

Objects that the GeoJSON decoder can return.

