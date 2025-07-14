

- MapKit
-  MapInteractionModes 

Structure

# MapInteractionModes

Options that indicate the user interactions that the map responds to.

MapKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct MapInteractionModes
```

## Overview

A person can’t interact with a map if the option set is empty.

## Topics

### Declared interaction modes

static let all: MapInteractionModes

The map allows all interaction modes.

static let pan: MapInteractionModes

The map allows a person to pan around to different areas of the map.

static let zoom: MapInteractionModes

The map allows people to zoom in or out on map locations.

static let pitch: MapInteractionModes

The map allows people to set the map’s pitch to view the map from different angles.

static let rotate: MapInteractionModes

The map allows people to rotate the map.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a map

init(bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?)

Creates a new, empty map with the bounds, interaction modes, and scope you provide.

init&lt;C>(bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?, content: () -> C)

Creates a new map with the bounds, interaction modes, scope, and content you provide.

init(bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?)

Creates a new, empty map with the bounds, interaction modes, a binding to a map feature, and scope you provide.

init&lt;SelectedValue>(bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;SelectedValue?>, scope: Namespace.ID?)

Creates a new, empty map with the bounds, interaction modes, the selected map feature, and scope you provide.

init&lt;C>(bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the bounds, interaction modes, selected map feature, scope, and map content you provide.

init&lt;SelectedValue, C>(bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;SelectedValue?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the bounds, interaction modes, selected value, scope, and map content you provide.

init(initialPosition: MapCameraPosition, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?)

Creates a new, empty map with the initial camera position, bounds, interaction modes, and scope you provide.

init&lt;C>(initialPosition: MapCameraPosition, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, scope, and map content you provide.

init(initialPosition: MapCameraPosition, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?)

Creates a new, empty map with the initial camera position, bounds, interaction modes, selected map feature, and scope you provide.

init&lt;C>(initialPosition: MapCameraPosition, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, selected map feature, scope, and content you provide.

init&lt;SelectedValue, C>(initialPosition: MapCameraPosition, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;SelectedValue?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, selected map feature, scope, and content you provide.

init(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?)

Creates a new, empty map with the initial camera position, bounds, interaction modes, and scope you provide.

init&lt;C>(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, scope, and content you provide.

init(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?)

Creates a new map with the initial camera position, bounds, interaction modes, scope, and content you provide.

init&lt;C>(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, selected feature, scope, and content you provide.

