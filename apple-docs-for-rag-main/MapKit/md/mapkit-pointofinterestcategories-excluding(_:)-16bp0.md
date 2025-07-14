

- MapKit
- PointOfInterestCategories
-  excluding(\_:) 

Type Method

# excluding(\_:)

Show all points of interest except those belonging to certain categories using the array you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func excluding(_ categories: [MKPointOfInterestCategory]) -> PointOfInterestCategories
```

## Parameters 

`categories`  

An array of points of interest categories to exclude.

## Return Value

Returns a set of point of interest categories to exclude.

## See Also

### Modifying the categories to include or exclude

static func excluding(MKPointOfInterestCategory...) -> PointOfInterestCategories

Show all points of interest except those belonging to certain categories using the list you provide.

static func including([MKPointOfInterestCategory]) -> PointOfInterestCategories

Show only points of interest belonging to certain categories from the provided array.

static func including(MKPointOfInterestCategory...) -> PointOfInterestCategories

Show only points of interest belonging to certain categories from the provided list.

