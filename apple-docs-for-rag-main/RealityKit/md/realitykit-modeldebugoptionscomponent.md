

- RealityKit
-  ModelDebugOptionsComponent 

Structure

# ModelDebugOptionsComponent

A component that changes how RealityKit renders its entity to help with debugging.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
struct ModelDebugOptionsComponent
```

## Overview

Attaching a `ModelDebugOptionsComponent` to a ModelEntity tells RealityKit to change the way it renders that entity based on a specified visualizationMode. This component isolates individual parts of the rendering process, such as the entity’s transparency or roughness, and displays surface color to help identify visual anomalies.

To use this component, create a `ModelDebugOptionsComponent` and set its visualizationMode to the desired value. Then, set the component as the entity’s modelDebugOptions property:

```
if let robot = anchor.findEntity(named: "Robot") as? ModelEntity {
    let component = ModelDebugOptionsComponent(visualizationMode: .normal)
    robot.modelDebugOptions = component
}
```

For more information on the visualization modes supported by `ModelDebugOptionsComponent`, see ModelDebugOptionsComponent.VisualizationMode.

### Attach a debug component to an entity

To attach a debug component to a particular entity, traverse the entity tree while passing the component to each child:

```
// Traverse the entity tree to attach a certain debug mode through components.
func attachDebug(entity: Entity, debug: ModelDebugOptionsComponent) {
    entity.components.set(debug)
    for child in entity.children {
        attachDebug(entity: child, debug: debug)
    }
}
// Respond to a button or UI element.
func debugLightingDiffuseButtonCallback() {
    let debugComponent = ModelDebugOptionsComponent(
        visualizationMode: .lightingDiffuse
    )
    attachDebug(entity: model, debug: debugComponent)
}
```

### Attach a debug component to a trait

To attach a debug component based on a trait, traverse the entity tree while checking for HasModel adoption:

```
func attachDebug(entity: Entity, debug: ModelDebugOptionsComponent) {
    if let model = entity as? ModelEntity {
        model.visualizationMode = debug
    }
    for child in entity.children {
        attachDebug(entity: child, debug: debug)
    }
}
// Respond to a button or UI element.
func debugLightingDiffuseButtonCallback() {
    let debugComponent = ModelDebugOptionsComponent(
        visualizationMode: .lightingDiffuse
    )
    attachDebug(entity: model, debug: debugComponent)
}
```

## Topics

### Creating model debug options components

init(visualizationMode: ModelDebugOptionsComponent.VisualizationMode)

Creates a component that isolates a portion of the rendering process and displays it as the entity’s surface texture.

### Setting the visualization mode

var visualizationMode: ModelDebugOptionsComponent.VisualizationMode

The part of the rendering process to display as the entity’s surface texture.

enum VisualizationMode

A mode that specifies the portion of the rendering process to isolate and display for debugging.

### Registering the component

static func registerComponent()

Registers a new component type.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Render configuration

struct ModelSortGroupComponent

A component that configures the rendering order for an entity’s model.

struct ModelSortGroup

A group that you assign to multiple entities to tell the renderer what order and how to render the entities in the group.

struct OpacityComponent

A component that controls the opacity of an entity and its descendants.

struct AdaptiveResolutionComponent

A component that provides the suggested pixels per meter necessary to render an object.

