

- MapKit JS
-  AnnotationConstructorOptions 

Structure

# AnnotationConstructorOptions

An object that contains options for creating annotation features.

MapKit JS 5.0+

``` source
dictionary AnnotationConstructorOptions {
 string title;
 string subtitle;
 string accessibilityLabel;
 Object data;
 boolean draggable;
 boolean visible;
 boolean enabled;
 boolean selected;
 boolean calloutEnabled;
 boolean animates;
 string appearanceAnimation;
 DOMPoint anchorOffset;
 DOMPoint calloutOffset;
 AnnotationCalloutDelegate callout;
 Object size;
 number displayPriority;
 string collisionMode;
 mapkit.Padding padding;
 string clusteringIdentifier;
 Place place;
 string id;
};
```

## Overview

Use AnnotationConstructorOptions when you need to create a custom view to provide features beyond those that the mapkit.ImageAnnotation object provides.

## Topics

### Creating data and titles

data

Data that you define and assign to the annotation.

title

The text to display in the annotation’s callout.

subtitle

The text to display as a subtitle on the second line of an annotation’s callout.

accessibilityLabel

Accessibility text for the annotation.

### Setting position and appearance attributes

anchorOffset

The offset, in CSS pixels, of the element from the bottom center.

appearanceAnimation

A CSS animation that runs when the annotation appears on the map.

displayPriority

A hint the map uses to prioritize displaying the annotation.

padding

Spacing to add around the annotation when showing items.

size

The desired dimensions of the annotation, in CSS pixels.

visible

A Boolean value that determines whether the annotation is visible or hidden.

### Creating interaction behavior

animates

A Boolean value that determines whether the map animates the annotation.

draggable

A Boolean value that determines whether the user can drag the annotation.

enabled

A Boolean value that determines whether the annotation responds to user interaction.

selected

A Boolean value that determines whether the map displays the annotation in a selected state.

place

An object that allows a custom annotation to potentially supecede a point of interest at the same map coordinates.

### Creating callouts

callout

A delegate that enables you to customize the annotation’s callout.

calloutEnabled

A Boolean value that determines whether the map shows a callout.

calloutOffset

The offset, in CSS pixels, of a callout from the top center of the element.

### Grouping annotations

clusteringIdentifier

An identifier for grouping annotations into the same cluster.

collisionMode

A mode that determines the shape of the collision frame.

id

A Place ID that uniquely identifies a feature.

## See Also

### Creating an annotation

mapkit.Annotation

Creates a new annotation given its location and initialization options.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

addEventListener

Adds an event listener to handle events that user interactions with annotations trigger.

removeEventListener

Removes an event listener.

