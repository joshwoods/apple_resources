

- MapKit
-  MKClusterAnnotation 

Class

# MKClusterAnnotation

An annotation that groups two or more distinct annotations into a single entity.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MKClusterAnnotation
```

## Overview

A cluster annotation object stands in for the group of annotations. Cluster views promote legibility of the underlying annotations by displaying a single annotation that takes it’s title from one annotation and includes a subtitle that indicates how many additional annotations belong to the group.

MapKit automatically creates cluster annotations when two or more annotation views group too closely together on the map surface. To customize the cluster annotations that display on your map, implement the mapView(_:clusterAnnotationForMemberAnnotations:) method in your map’s delegate.

## Topics

### Creating a cluster annotation

init(memberAnnotations: [any MKAnnotation])

Creates a cluster annotation with the specified individual annotations.

### Getting the cluster attributes

var title: String?

The title string to display for the group of annotations.

var subtitle: String?

The subtitle string to display for the group of annotations.

### Getting the annotations

var memberAnnotations: [any MKAnnotation]

The annotations that the cluster contains.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- NSObjectProtocol

## See Also

### Grouped annotations

Decluttering a Map with MapKit Annotation Clustering

Enhance the readability of a map by replacing overlapping annotations with a clustering annotation view.

