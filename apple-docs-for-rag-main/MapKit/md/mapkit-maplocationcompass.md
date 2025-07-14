

- MapKit
-  MapLocationCompass 

Structure

# MapLocationCompass

A view that displays a combined user location button and map compass.

MapKitSwiftUIwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct MapLocationCompass
```

## Overview

In watchOS 10 and later, this view displays a combined MapUserLocationButton and MapCompass control. When the map camera has a heading of zero (where north is up), this view shows the user location button. When the map camera is in a rotated state, it shows a compass.

Use `MapLocationCompass` in conjunction with Map as a standalone view, as shown in this example:

```
    struct LocationCompassTestView: View {
        @Namespace var mapScope

        var body: some View {
            VStack {
                Map(scope: mapScope)
                MapLocationCompass(scope: mapScope)
            }
            .mapScope(mapScope)
        }
    }
```

You can also use `MapLocationCompass` in conjunction with the `mapControls(_:)` modifier. For example:

```
    Map()
        .mapControls {
            MapLocationCompass()
        }
```

## Topics

### Creating a map loction compass

init(scope: Namespace.ID?)

Creates a new map location compass with the provided scope.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Map controls

struct MapCompass

A view that reflects the current orientation of the associated map.

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

