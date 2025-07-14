

- MapKit
-  MapCompass 

Structure

# MapCompass

A view that reflects the current orientation of the associated map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct MapCompass
```

## Overview

You can use `MapCompass` with a Map as a stand alone view, as shown in the following example:

```
    struct CompassButtonTestView: View {
        @Namespace var mapScope
        var body: some View {
        VStack {
                Map(scope: mapScope)
                MapCompass(scope: mapScope)
            }
            .mapScope(mapScope)
        }
    }
```

You can also use `MapCompass` with the `Map/mapControls(_:)`, modifier, as shown below:

```
    Map()
        .mapControls {
            MapCompass()
        }
```

Tapping the compass reorients the map so that North is at the top of the Map view.

## Topics

### Creating a map compass

init(scope: Namespace.ID?)

Creates a new map compass with the scope you specify.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Map controls

struct MapLocationCompass

A view that displays a combined user location button and map compass.

struct MapPitchSlider

A slider control that allows a person to change the pitch of the map.

struct MapPitchToggle

A button that sets the pitch of the associated map.

struct MapScaleView

Displays a legend with distance information for the associated map.

struct MapUserLocationButton

A button that sets the framing of the associated map to the user location.

struct MapZoomStepper

Buttons a person uses to adjust the zoom level of the map.

