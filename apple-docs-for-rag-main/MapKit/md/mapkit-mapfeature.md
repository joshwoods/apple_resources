

- MapKit
-  MapFeature 

Structure

# MapFeature

A tappable map feature.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapFeature
```

## Overview

Tappable map features can include single points of interest, such as hotels and restaurants, a territory, or a physical map feature such as an ocean, basin, river, or mountain range.

## Topics

### Accessing the feature’s properties

var kind: MapFeature.FeatureKind

The kind of feature represented by the map feature.

struct FeatureKind

The kind of feature represented by a map feature.

var coordinate: CLLocationCoordinate2D

The coordinate of the map feature.

var title: String?

The title of the map feature.

var backgroundColor: Color?

The background color associated with the map feature.

var image: Image?

An image associated with the map feature.

var pointOfInterestCategory: MKPointOfInterestCategory?

The point of interest category of the map feature.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Map features

struct MapSelection

A value representing a selected feature on a map.

protocol MapSelectable

