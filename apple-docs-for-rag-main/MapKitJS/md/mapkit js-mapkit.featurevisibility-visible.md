

- MapKit JS
- mapkit.FeatureVisibility
-  Visible 

Enumeration Case

# Visible

A constant indicating that the feature is always visible.

MapKit JS 5.0+

``` source
const string Visible;
```

## Discussion

Use `mapkit.FeatureVisibility.Visible` to always show adaptive map controls, such as the compass and scale, regardless of the map’s current state. You can show or hide controls that aren’t adaptive by setting map properties to `true` or `false`, respectively.

The following example shows how to always show the compass and the user location control:

```
// Create a map.
var map = new mapkit.Map("my-map-element-id");

// Always show the compass, regardless of the map state. 
map.showsCompass = mapkit.FeatureVisibility.Visible;

// Show the user location control. 
map.showsUserLocationControl = true;
```

## See Also

### Feature visibility values

Adaptive

A constant indicating that feature visibility adapts to the current map state.

Hidden

A constant indicating that the feature is always hidden.

