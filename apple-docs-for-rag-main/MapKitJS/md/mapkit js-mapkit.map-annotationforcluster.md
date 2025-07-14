

- MapKit JS
- mapkit.Map
-  annotationForCluster 

Instance Method

# annotationForCluster

A delegate method for modifying an annotation that represents a group of annotations that the framework combines into a cluster.

MapKit JS 5.0+

``` source
void annotationForCluster(
 mapkit.Annotation clusterAnnotation
);
```

## Parameters 

`clusterAnnotation`  

An annotation that represents a group of annotations that MapKit JS combines into a cluster.

## Mentioned in 

Clustering annotations

## Discussion

MapKit JS invokes this delegate method when it creates a cluster annotation, or when a member annotation within the cluster changes.

You can return any of the following:

- The same cluster annotation with its properties, such as title or subtitle, modified.

- A new annotation, such as an image annotation, to represent the cluster.

- No return value. If you don’t return an annotation, MapKit JS uses the default annotation. You don’t need to return a default annotation even if you modify it (as the following code example shows for the cities cluster); the map displays the modifications.

The following example creates annotation clusters for cities and parks:

```
map.addAnnotations(cities.map(city =>
    new mapkit.MarkerAnnotation(city.coordinate, {
        title: city.name,
        subtitle: city.population,
        glyphImage: city.landmarkImage,
        displayPriority: Math.max(city.population / 10000, 1000),
        clusteringIdentifier: "city"
    })
));

map.addAnnotations(parks.map(park =>
    new mapkit.ImageAnnotation(park.coordinate, {
        title: park.name,
        url: { 1: park.image },
        displayPriority: 250,
        clusteringIdentifier: "park"
    })
));

map.annotationForCluster = function(clusterAnnotation) {
    if (clusterAnnotation.clusteringIdentifier === "city") {
        clusterAnnotation.title = "Cities";
        clusterAnnotation.subtitle = clusterAnnotation.memberAnnotations
            .reduce((total, clusterAnnotation) => total + clusterAnnotation.population, 0);
    } else if (clusterAnnotation.clusteringIdentifier === "park") {
        return new mapkit.ImageAnnotation(clusterAnnotation.coordinate, {
            title: "Parks",
            url: { 1: "tree.png" }
        });
    }
};
```

For more information, see Clustering annotations.

## See Also

### Annotating the map

annotations

An array of all the annotations on the map.

selectedAnnotation

The selected annotation.

annotationsInMapRect

Returns the list of annotation objects within the specified map rectangle.

addAnnotation

Adds an annotation to the map.

addAnnotations

Adds an array of annotations to the map.

removeAnnotation

Removes an annotation from the map.

removeAnnotations

Removes multiple annotations from the map.

