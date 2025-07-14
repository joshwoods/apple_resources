

- MapKit
- MKAnnotationView
-  cluster 

Instance Property

# cluster

The clustering annotation view that replaces the annotation view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
weak var cluster: MKAnnotationView? { get }
```

## Discussion

When the map is displaying this annotation view, the value of this property is `nil`.

## See Also

### Clustering annotation views

Decluttering a Map with MapKit Annotation Clustering

Enhance the readability of a map by replacing overlapping annotations with a clustering annotation view.

var clusteringIdentifier: String?

An identifier that determines whether the annotation view participates in clustering.

