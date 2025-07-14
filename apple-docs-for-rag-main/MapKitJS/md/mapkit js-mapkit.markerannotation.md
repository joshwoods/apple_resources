

- MapKit JS
-  mapkit.MarkerAnnotation 

Class

# mapkit.MarkerAnnotation

An annotation that displays a balloon-shaped marker at the designated location.

MapKit JS 5.0+

``` source
interface mapkit.MarkerAnnotation
```

## Mentioned in 

MapKit JS 5

## Overview

A *marker* is a balloon-shaped annotation that contains a glyph or text. On the map, the marker appears when its coordinate is in view.

The following example shows a customized marker that specifies a color for the balloon background and the glyph, and provides custom glyph images. Color properties accept either a color name, here “brown” and “green”, or the equivalent hexadecimal color value such as “`#A52A2A`” and “`#008000`”, respectively. Or, you can use a specific color that matches your apps specific design. For more information on standardized colors, see the CSS working group’s list of common color names and values.

```
var portland = new mapkit.Coordinate(45.5231, -122.6765);
var customMarker = new MarkerAnnotation(portland, {
    color: "green",
    glyphColor: "brown",
    glyphImage: { 1: "glyphImage.png" },
    selectedGlyphImage: { 1: "detailedIcon.png", 2: "detailedIcon_2x.png", 3: "detailedIcon_3x.png" }
});
```

The following example shows a marker annotation with a custom callout implemented by the callout delegate. In this example, the annotation is a dot when selected because selectedGlyphImage isn’t used.

```
var calloutDelegate = {
    calloutRightAccessoryForAnnotation: function() {
        var accessoryViewRight = document.createElement("a");
        accessoryViewRight.className = "right-accessory-view";
        accessoryViewRight.href = "https://www.nps.gov/stli/index.htm";
        accessoryViewRight.target = "_blank";
        accessoryViewRight.appendChild(document.createTextNode("ⓘ"));

        return accessoryViewRight;
    }
};

var annotation = new mapkit.MarkerAnnotation(new mapkit.Coordinate(40.6892, -74.0445), {
    title: "Title",
    subtitle: "Subtitle",
    callout: calloutDelegate
});
```

------------------------------------------------------------------------

## Topics

### Creating a marker annotation

mapkit.MarkerAnnotation

Creates a marker annotation at the coordinate location with provided options.

MarkerAnnotationConstructorOptions

An object containing the options that create a marker annotation.

### Setting visibility

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

titleVisibility

A value that determines the behavior of the title’s visibility.

mapkit.FeatureVisibility

Constants indicating the visibility of different adaptive map features.

### Setting appearance

color

The background color of the balloon.

glyphColor

The fill color of the glyph.

### Setting the glyph image and text

glyphText

The text to display in the marker balloon.

glyphImage

The image to display in the marker balloon.

selectedGlyphImage

The image to display in the marker balloon when the user selects the marker.

## Relationships

### Inherited By

- mapkit.Annotation

