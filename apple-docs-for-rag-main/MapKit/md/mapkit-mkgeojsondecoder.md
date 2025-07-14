

- MapKit
-  MKGeoJSONDecoder 

Class

# MKGeoJSONDecoder

An object that decodes GeoJSON objects into MapKit types.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKGeoJSONDecoder
```

## Overview

The GeoJSON decoder returns objects that conform to the MKGeoJSONObject protocol.

## Topics

### Decoding GeoJSON objects

func decode(Data) throws -> [any MKGeoJSONObject]

Decodes the provided data into native MapKit types that a map can display.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Geographical features

Displaying an Indoor Map

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest.

class MKGeoJSONFeature

The decoded representation of a GeoJSON feature.

protocol MKGeoJSONObject

Objects that the GeoJSON decoder can return.

