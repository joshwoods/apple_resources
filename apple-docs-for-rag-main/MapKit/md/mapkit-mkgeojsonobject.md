

- MapKit
-  MKGeoJSONObject 

Protocol

# MKGeoJSONObject

Objects that the GeoJSON decoder can return.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol MKGeoJSONObject : NSObjectProtocol
```

## Overview

Classes that conform to this protocol represent the types that the GeoJSON decoder can return.

There’s no reason to create your own classes that conform to this protocol; only MapKit can define classes that the GeoJSON decoder uses.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MKGeoJSONFeature
- MKGeodesicPolyline
- MKMultiPoint
- MKMultiPolygon
- MKMultiPolyline
- MKPointAnnotation
- MKPolygon
- MKPolyline

## See Also

### Geographical features

Displaying an Indoor Map

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest.

class MKGeoJSONDecoder

An object that decodes GeoJSON objects into MapKit types.

class MKGeoJSONFeature

The decoded representation of a GeoJSON feature.

