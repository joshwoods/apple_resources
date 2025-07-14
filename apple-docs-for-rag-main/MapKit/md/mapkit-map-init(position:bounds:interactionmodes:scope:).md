

- MapKit
- Map
-  init(position:bounds:interactionModes:scope:) 

Initializer

# init(position:bounds:interactionModes:scope:)

Creates a new, empty map with the initial camera position, bounds, interaction modes, and scope you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    position: Binding,
    bounds: MapCameraBounds? = nil,
    interactionModes: MapInteractionModes = .all,
    scope: Namespace.ID? = nil
) where Content == MapContentView
```

Available when `Content` conforms to `View`.

## Parameters 

`position`  

The initial MapCameraPosition.

`bounds`  

The MapCameraBounds that define the camera’s view of the map.

`interactionModes`  

The MapInteractionModes that describe ways a person can interact with the map.

`scope`  

The map’s Namespace.ID.

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

init&lt;C>(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, scope, and content you provide.

init(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?)

Creates a new map with the initial camera position, bounds, interaction modes, scope, and content you provide.

init&lt;C>(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;MapFeature?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, selected feature, scope, and content you provide.

init&lt;SelectedValue, C>(position: Binding&lt;MapCameraPosition>, bounds: MapCameraBounds?, interactionModes: MapInteractionModes, selection: Binding&lt;SelectedValue?>, scope: Namespace.ID?, content: () -> C)

Creates a new map with the initial camera position, bounds, interaction modes, selected feature, scope, and content you provide.

