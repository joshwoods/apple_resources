

- MapKit
- PointOfInterestCategories
-  including(\_:) 

Type Method

# including(\_:)

Show only points of interest belonging to certain categories from the provided list.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func including(_ categories: MKPointOfInterestCategory...) -> PointOfInterestCategories
```

## Parameters 

`categories`  

The points of interest categories to include.

## Return Value

Returns the points of interest to include.

## See Also

### Modifying the categories to include or exclude

static func excluding([MKPointOfInterestCategory]) -> PointOfInterestCategories

Show all points of interest except those belonging to certain categories using the array you provide.

static func excluding(MKPointOfInterestCategory...) -> PointOfInterestCategories

Show all points of interest except those belonging to certain categories using the list you provide.

static func including([MKPointOfInterestCategory]) -> PointOfInterestCategories

Show only points of interest belonging to certain categories from the provided array.

