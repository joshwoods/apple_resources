

- MapKit JS
-  mapkit.Map.MapTypes 

Enumeration

# mapkit.Map.MapTypes

Constants representing the type of map to display.

MapKit JS 5.0+

``` source
interface mapkit.Map.MapTypes {
 const string Standard;
 const string MutedStandard;
 const string Hybrid;
 const string Satellite;
};
```

## Mentioned in 

Handling map events

## Topics

### Map type values

Hybrid

A satellite image of the area with road and road name layers on top.

MutedStandard

A street map that emphasizes your data over the underlying map details.

Satellite

A satellite image of the area.

Standard

A street map that shows the position of all roads and some road names.

## See Also

### Configuring the map’s appearance

colorScheme

The map’s color scheme when displaying standard or muted standard map types.

mapkit.Map.ColorSchemes

Constants indicating the color scheme of the map.

distances

The system of measurement that displays on the map.

mapkit.Map.Distances

Constants indicating the system of measurement that displays on the map.

mapType

The type of data that the map displays.

padding

The map’s inset margins.

pointOfInterestFilter

The filter that determines the points of interest that display on the map.

showsPointsOfInterest

A Boolean value that determines whether the map displays points of interest.

showItems

Adjusts the map’s visible region to bring the specified overlays and annotations into view.

MapShowItemsOptions

Options that determine the map parameters to use when showing items.

tintColor

The CSS color that MapKit JS uses for user interface controls on the map.

