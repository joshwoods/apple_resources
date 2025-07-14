

- MapKit JS
-  mapkit.Annotation 

Class

# mapkit.Annotation

The base annotation object for creating custom annotations.

MapKit JS 5.0+

``` source
interface mapkit.Annotation
```

## Mentioned in 

Handling map events

## Overview

An annotation represents data that you want to display on the map’s surface. Associate each annotation with a coordinate on the map. It’s rare that you need to create a mapkit.Annotation object. Use the more common extended objects, mapkit.MarkerAnnotation and mapkit.ImageAnnotation instead.

Use mapkit.Annotation when you need to customize a view in a way that you can’t accomplish with mapkit.ImageAnnotation.

The examples below create a custom annotation using a person’s initials to show them on the map. The following CSS style encloses the initials in a gray circle:

```
.circle-annotation {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    color: #FFF;
    background-color: #CCC;
    text-align: center;
    line-height: 32px;
}
```

The following code creates the annotation:

```
var people = [
    { title: "Juan Chavez",
      coordinate: new mapkit.Coordinate(37.3349, -122.0090201),
      role: "developer",
      building: "HQ" },
    { title: "Anne Johnson",
      coordinate: new mapkit.Coordinate(37.722319, -122.434979),
      role: "manager",
      building: "HQ" }
];

var factory = function(coordinate, options) {
    var div = document.createElement("div"),
        name = options.title,           // "Juan Chavez"
        parts = name.split(' ');        // ["Chavez", "Juan"]
    div.textContent = parts[0].charAt(0) + parts[1].charAt(0);    // "JA"
    div.className = "circle-annotation";
    return div;
};

people.forEach(function(person) {
    var options = {
        title: person.title,
        data: { role: person.role, building: person.building }
    };
    var annotation = new mapkit.Annotation(person.coordinate, factory, options);
    map.addAnnotation(annotation);
});
```

## Topics

### Creating an annotation

mapkit.Annotation

Creates a new annotation given its location and initialization options.

AnnotationConstructorOptions

An object that contains options for creating annotation features.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

addEventListener

Adds an event listener to handle events that user interactions with annotations trigger.

removeEventListener

Removes an event listener.

### Getting the map and element

map

The map that the framework adds the annotation to.

element

The annotation’s element in the DOM.

### Getting and setting data, titles, and the accessibility label

data

Data that you define that’s specific to an annotation.

title

The text to display in the annotation’s callout.

subtitle

The text to display as a subtitle on the second line of an annotation’s callout.

accessibilityLabel

Accessibility text for the annotation.

### Getting and setting annotation appearance

coordinate

The annotation’s coordinate.

anchorOffset

An offset that changes the annotation’s default anchor point.

appearanceAnimation

A CSS animation that runs when the annotation appears on the map.

displayPriority

A numeric hint that the map uses to prioritize how it displays annotations.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

padding

Spacing to add around the annotation when showing items.

size

The desired dimensions of the annotation, in CSS pixels.

visible

A Boolean value that determines whether the annotation is visible or hidden.

### Getting and setting interaction behavior

animates

A Boolean value that determines whether the framework animates the annotation.

draggable

A Boolean value that determines whether the user can drag the annotation.

selected

A Boolean value that indicates whether the map shows the annotation in a selected state.

enabled

A Boolean value that determines whether the annotation responds to user interaction.

### Managing callouts

callout

A delegate that enables you to customize the annotation’s callout.

calloutEnabled

A Boolean value that determines whether the map shows an annotation’s callout.

calloutOffset

An offset that changes the annotation callout’s default placement.

### Managing clustering

memberAnnotations

An array of annotations that the framework groups together in a cluster.

clusteringIdentifier

An identifier for grouping annotations into the same cluster.

collisionMode

A mode that determines the shape of the collision frame.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

### Managing selection accessories

selectionAccessory

An accessory that displays place information when a person selects a place.

selectionAccessoryOffset

An offset that changes the selection accessory’s default anchor point.

## See Also

### Annotations

Clustering annotations

Combine multiple annotations into a single clustered annotation.

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

