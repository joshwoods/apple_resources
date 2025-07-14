

- MapKit
-  MapPitchToggle 

Structure

# MapPitchToggle

A button that sets the pitch of the associated map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
struct MapPitchToggle
```

## Overview

The `MapPitchToggle` control sets the pitch of the associated map to a pleasing angle if flat, or returns the map to flat if pitched.

You can use this control in conjunction with Map as a standalone view, as this example shows:

```
    struct MyMapView: View {
        @Namespace var mapScope

        var body: some View {
            VStack {
                Map(scope: mapScope)
                MapPitchToggle(scope: mapScope)
            }
            .mapScope(mapScope)
        }
    }
```

Alternatively, use `MapPitchToggle` in conjunction with the `mapControls(_:)` modifier. For example:

```
    Map()
        .mapControls {
            MapPitchToggle()
        }
```

## Topics

### Creating a map pitch toggle

init(scope: Namespace.ID?)

Creates a new map pitch toggle control with the provided scope.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Map controls

struct MapCompass

A view that reflects the current orientation of the associated map.

struct MapLocationCompass

A view that displays a combined user location button and map compass.

struct MapPitchSlider

A slider control that allows a person to change the pitch of the map.

struct MapScaleView

Displays a legend with distance information for the associated map.

struct MapUserLocationButton

A button that sets the framing of the associated map to the user location.

struct MapZoomStepper

Buttons a person uses to adjust the zoom level of the map.

