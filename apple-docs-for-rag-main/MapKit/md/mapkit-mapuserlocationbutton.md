

- MapKit
-  MapUserLocationButton 

Structure

# MapUserLocationButton

A button that sets the framing of the associated map to the user location.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct MapUserLocationButton
```

## Overview

Use `MapUserLocationButton` in conjunction with Map as a stand alone view, as shown in this example:

```
    struct LocationButtonTestView: View {
        @Namespace var mapScope
        var body: some View {
            VStack {
                Map(scope: mapScope)
                MapUserLocationButton(scope: mapScope)
            }
            .mapScope(mapScope)
        }
    }
```

You can also use `MapUserLocationButton` in conjunction with the `Map/mapControls(_:)` modifier as shown in this example:

```
    Map()
        .mapControls {
            MapUserLocationButton()
        }
```

## Topics

### Creating a map user location button

init(scope: Namespace.ID?)

Creates a new user location button with the scope you specify.

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

struct MapPitchToggle

A button that sets the pitch of the associated map.

struct MapScaleView

Displays a legend with distance information for the associated map.

struct MapZoomStepper

Buttons a person uses to adjust the zoom level of the map.

