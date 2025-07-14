

- MapKit
-  MapZoomStepper 

Structure

# MapZoomStepper

Buttons a person uses to adjust the zoom level of the map.

MapKitSwiftUIMac Catalyst 14.0+macOS 14.0+

``` source
@MainActor @preconcurrency
struct MapZoomStepper
```

## Overview

You typically use MapZoomStepper with Map as a stand alone view, as shown in the following example:

```
    struct ZoomStepperTestView: View {
        @Namespace var mapScope
        var body: some View {
            VStack {
                Map(scope: mapScope)
                MapZoomStepper(scope: mapScope)
            }
            .mapScope(mapScope)
        }
    }
```

You can also use a MapZoomStepper in conjunction with the `Map/mapControls(_:)` modifier, as show in here:

```
    Map()
        .mapControls {
            MapZoomStepper()
        }
```

## Topics

### Creating a zoom stepper

init(scope: Namespace.ID?)

Creates a new zoom stepper with the scope you specify.

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

struct MapUserLocationButton

A button that sets the framing of the associated map to the user location.

