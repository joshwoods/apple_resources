

- MapKit
-  MKAnnotation 

Protocol

# MKAnnotation

An interface for associating your content with a specific map location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol MKAnnotation : NSObjectProtocol
```

## Overview

An object that adopts this protocol manages the data that you want to display on the map surface. It doesn’t provide the visual representation that the map displays. Instead, your map view’s delegate provides the MKAnnotationView objects necessary to display the content of your annotations. When you want to display content at a specific point on the map, add an annotation object to the map view. When the annotation’s coordinate is visible on the map, the map view asks its delegate to provide an appropriate view to display any content associated with the annotation. You implement the mapView(_:viewFor:) method of the delegate to provide that view.

An object that adopts this protocol needs to implement the coordinate property. The other methods of this protocol are optional.

## Topics

### Position attributes

var coordinate: CLLocationCoordinate2D

The center point (specified as a map coordinate) of the annotation.

**Required**

### Title attributes

var title: String?

The string containing the annotation’s title.

var subtitle: String?

The string containing the annotation’s subtitle.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MKOverlay

### Conforming Types

- MKCircle
- MKClusterAnnotation
- MKGeodesicPolyline
- MKMapFeatureAnnotation
- MKMapItemAnnotation
- MKMultiPoint
- MKMultiPolygon
- MKMultiPolyline
- MKPlacemark
- MKPointAnnotation
- MKPolygon
- MKPolyline
- MKShape
- MKTileOverlay
- MKUserLocation

## See Also

### Shared behavior

class MKPlacemark

A user-friendly description of a location on the map.

class MKAnnotationView

The visual representation of one of your annotation objects.

