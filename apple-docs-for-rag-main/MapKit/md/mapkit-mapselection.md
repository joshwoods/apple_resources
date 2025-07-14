

- MapKit
-  MapSelection 

Structure

# MapSelection

A value representing a selected feature on a map.

MapKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MapSelection where SelectionValue : Hashable
```

## Topics

### Creating a map selection

init(SelectionValue)

Creates a map selection with a tag.

### Getting the properties

var value: SelectionValue?

The selection of the given tag value.

## Relationships

### Conforms To

- Equatable
- Hashable
- MapSelectable

## See Also

### Map features

struct MapFeature

A tappable map feature.

protocol MapSelectable

