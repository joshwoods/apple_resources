

- MapKit JS
-  mapkit.Padding 

Class

# mapkit.Padding

The values that define content padding within the map view frame.

MapKit JS 5.0+

``` source
interface mapkit.Padding
```

## Overview

Use padding to define edge insets on the map. MapKit JS then uses these insets when it positions items on the map, such as the map controls or annotations. For example, if you want to add your own control on top of the map and ensure that the map doesn’t position annotations underneath it, you can add padding to the map and then position your control within the padded area.

You can use a `Padding` object when setting the map’s padding property or as an option of showItems. Positive values add padding to the inside edges of the map. MapKit JS clips negative values to `0`.

## Topics

### Creating padding

mapkit.Padding

Creates a padding object and initializes its inset margin properties.

PaddingConstructorOptions

Initial values of the edge insets for padding.

### Controlling the map’s padding

bottom

The amount of padding, in CSS pixels, to inset the map from the bottom edge.

left

The amount of padding, in CSS pixels, to inset the map from the left edge.

right

The amount of padding, in CSS pixels, to inset the map from the right edge.

top

The amount of padding, in CSS pixels, to inset the map from the top edge.

## See Also

### Map view customization

mapkit.FeatureVisibility

Constants indicating the visibility of different adaptive map features.

