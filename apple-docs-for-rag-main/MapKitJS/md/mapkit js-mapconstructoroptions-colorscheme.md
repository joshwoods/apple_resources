

- MapKit JS
- MapConstructorOptions
-  colorScheme 

Instance Property

# colorScheme

The map’s color scheme when displaying standard or muted standard map types.

MapKit JS 5.12+

``` source
attribute string colorScheme;
```

## Discussion

This property accepts a property from mapkit.Map.ColorSchemes to determine whether the map displays with a dark or light theme when Standard or MutedStandard are the configured mapType. The default is Light.

The grid, user location accuracy ring, labels for marker annotations, and controls of the map change appearance to complement the Dark Mode style.

## See Also

### Setting the map’s appearance and controls

mapType

The type of data that the map view displays.

padding

The map’s inset margins.

showsMapTypeControl

A Boolean value that determines whether to display a control that lets users choose the map type.

isRotationEnabled

A Boolean value that determines whether the user may rotate the map using the compass control or a rotate gesture.

showsCompass

A feature visibility setting that determines when the compass is visible.

isZoomEnabled

A Boolean value that determines whether the user may zoom in and out on the map using pinch gestures or the zoom control.

showsZoomControl

A Boolean value that determines whether to display a control for zooming in and zooming out on a map.

isScrollEnabled

A Boolean value that determines whether the user may scroll the map with a pointing device or gestures on a touchscreen.

showsScale

A feature visibility setting that allows you to determine when to display the map’s scale.

