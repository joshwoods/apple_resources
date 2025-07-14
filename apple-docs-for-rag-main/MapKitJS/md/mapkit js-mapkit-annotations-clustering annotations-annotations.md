

- MapKit JS
- mapkit
- Annotations
-  Clustering annotations 

Article

# Clustering annotations

Combine multiple annotations into a single clustered annotation.

## Overview

Annotations display coordinate-specific data on a map, typically in the form of markers or images. To declutter annotation-heavy maps, MapKit JS supports *annotation clustering*. As the user zooms out on a map that contains annotations, MapKit JS groups individual annotations into a *cluster annotation* if they collide and if they share the same clusteringIdentifier.

The cluster annotation’s memberAnnotations property lists the individual annotations within the cluster. By default, a cluster annotation’s marker displays its member count.

MapKit JS creates cluster annotations automatically. Although you can’t instantiate a cluster annotation, you can customize the look of cluster annotations by providing a delegate method, annotationForCluster, to the map.

### Understand the annotations arrays

Although visible on a map, cluster annotations aren’t members of the map’s annotations array. The annotations that make up the cluster do belong to the annotations array, however, even if they’re not individually visible on the map. For example, the following figure shows a map with annotations A, B, C, D, and E:

If the user zooms out so A, B, and C overlap on the map, the annotations combine to create cluster annotation Q, as in the following figure:

The map displays annotations Q, D, and E, and the resulting annotation arrays are:

- `Q.memberAnnotations = [A, B, C];`

- `map.annotations = [A, B, C, D, E];`

### Set cluster annotation properties

Cluster annotations have the same properties as other annotations, but you can’t set some values, including coordinate, clusteringIdentifier, and draggable. Other values have specific defaults as the following table shows:

| Property | Default for clustering | Description |
|----|----|----|
| title | The `title` of the member annotation with the highest priority. | The annotation title text. |
| subtitle | “`+N` more”, where `N + 1` is the number of member annotations. | The annotation subtitle text. |
| coordinate | The average of the member annotation coordinates. | The annotation’s coordinate. The system automatically sets the coordinate of a cluster annotation to the average of all of the contained member annotation coordinates. You can’t change this value; therefore, the user can’t ever drag a cluster annotation. |
| glyphText | `N + 1` (the number of member annotations). | The annotation glyph text. |
| draggable | `false` | Determines whether the user may drag the annotation. You can’t modify this property. |
| memberAnnotations | NA | A flat array containing all annotations within the cluster annotation. Only cluster annotations have a `memberAnnotations` property. You can’t modify this property. |
| clusteringIdentifier | `null` | A shared identifier for all of the member annotations. An annotation needs a `clusteringIdentifier` to be part of an annotation cluster. |

## See Also

### Annotations

mapkit.Annotation

The base annotation object for creating custom annotations.

AnnotationCalloutDelegate

Methods for customizing the behavior and appearance of an annotation callout.

mapkit.PlaceAnnotation

An annotation for a place.

mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

