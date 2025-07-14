

- MapKit JS
- mapkit.Overlay
-  style 

Instance Property

# style

Style properties to apply to the overlay.

MapKit JS 5.0+

``` source
attribute mapkit.Style style;
```

## Discussion

The following example shows a new style object replacing the current style properties for a circle overlay:

```
circleOverlay.style = new mapkit.Style({
    strokeColor: "#777",
    lineWidth: 3,
    fillColor: "#FFF",
    fillOpacity: .2
});
```

You can also change style properties individually, as this example shows:

```
circleOverlay.style.fillOpacity = .33;
circleOverlay.style.lineWidth = 4;
```

## See Also

### Setting overlay options

data

Custom data to associate with the overlay.

visible

A Boolean value that determines whether an overlay is visible.

enabled

A Boolean value that determines whether the overlay responds to user interaction.

selected

A Boolean value that indicates whether the user selects the overlay.

map

The map you add the overlay to.

