

- MapKit
- MKAnnotationView
-  clusteringIdentifier 

Instance Property

# clusteringIdentifier

An identifier that determines whether the annotation view participates in clustering.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var clusteringIdentifier: String? { get set }
```

## Discussion

The default value of this property is `nil`, which prevents MapKit from clustering the annotation view with other annotation views. Setting the property to a non-`nil` value enables it to participate in clustering.

Clustering occurs when there’s a collision between multiple annotation views with the same identifier on the map surface. MapKit removes the annotation views involved in the collision from the map view and replaces them with a clustering annotation view, which displays the title from one of the annotations and provides access to the other annotations.

## See Also

### Clustering annotation views

Decluttering a Map with MapKit Annotation Clustering

Enhance the readability of a map by replacing overlapping annotations with a clustering annotation view.

var cluster: MKAnnotationView?

The clustering annotation view that replaces the annotation view.

