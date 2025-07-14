

- MapKit
-  DynamicMapContent 

Protocol

# DynamicMapContent

A  type of view that generates views from an underlying collection of data.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
protocol DynamicMapContent : MapContent
```

## Topics

### Accessing the data

var data: Self.Data

The collection of underlying data.

**Required**

### Associated types

associatedtype Data : Collection

The type represents the data this protocol contains.

**Required**

## Relationships

### Inherits From

- MapContent

## See Also

### Protocols

protocol MapContent

A protocol used to construct map content such as controls, markers, and annotations.

struct MapContentBuilder

A result builder that creates map content from closures you provide.

struct MapContentView

A view that contains content that displays on a map at a specific position, and that responds to specific interactions you specify.

