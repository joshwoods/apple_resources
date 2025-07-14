

- MapKit
-  PointOfInterestCategories 

Structure

# PointOfInterestCategories

A structure you use to define points of interest to include or exclude on a map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct PointOfInterestCategories
```

## Topics

### Categories to include or exclude

static var all: PointOfInterestCategories

A list of all points of interest categories, both included and excluded.

static var excludingAll: PointOfInterestCategories

A list of point of interest categories to exclude from display on the map.

### Modifying the categories to include or exclude

static func excluding([MKPointOfInterestCategory]) -> PointOfInterestCategories

Show all points of interest except those belonging to certain categories using the array you provide.

static func excluding(MKPointOfInterestCategory...) -> PointOfInterestCategories

Show all points of interest except those belonging to certain categories using the list you provide.

static func including([MKPointOfInterestCategory]) -> PointOfInterestCategories

Show only points of interest belonging to certain categories from the provided array.

static func including(MKPointOfInterestCategory...) -> PointOfInterestCategories

Show only points of interest belonging to certain categories from the provided list.

## Relationships

### Conforms To

- Copyable
- ExpressibleByArrayLiteral

