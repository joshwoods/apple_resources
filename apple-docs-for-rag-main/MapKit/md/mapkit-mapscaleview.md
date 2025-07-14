

- MapKit
-  MapScaleView 

Structure

# MapScaleView

Displays a legend with distance information for the associated map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
struct MapScaleView
```

## Overview

You can use this with Map as a standalone view, for example:

```
    struct ScaleTestView: View {
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

The scale indicator grows and shrinks (although visually, its frame is static) based on the zoom level of the map. By default the leading edge remains anchored and the trailing edge moves as the scale changes. If the scale is trailing aligned, then it may be more visually appealing to anchor the `ScaleView` to the trailing edge

```
    ZStack(alignment: .trailing) {
        Map(mapScope)
        MapScaleView(anchorEdge: .trailing, scope: mapScope)
    }
    .mapScope(mapScope)
```

You can also use `MapScaleView` with the mapControls(_:) modifier, as shown in this example:

```
    Map()
        .mapControls {
            MapScaleView()
        }
```

## Topics

### Creating a map scale view

init(anchorEdge: HorizontalEdge, scope: Namespace.ID?)

Creates a map scale view.

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

struct MapUserLocationButton

A button that sets the framing of the associated map to the user location.

struct MapZoomStepper

Buttons a person uses to adjust the zoom level of the map.

