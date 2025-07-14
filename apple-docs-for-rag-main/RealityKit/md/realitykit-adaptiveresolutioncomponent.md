

- RealityKit
-  AdaptiveResolutionComponent 

Structure

# AdaptiveResolutionComponent

A component that provides the suggested pixels per meter necessary to render an object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct AdaptiveResolutionComponent
```

## Overview

Use the pixelsPerMeter property to proactively update your scene to disable expensive systems and high-resolution content that is far away.

Note

`pixelsPerMeter` is binned to protect user privacy.

## Topics

### Initializers

init()

Creates a new instance of the adaptive resolution component.

### Instance Properties

var pixelsPerMeter: Float

A read-only value representing the suggested pixels per meter necessary to render an object.

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

struct ModelDebugOptionsComponent

A component that changes how RealityKit renders its entity to help with debugging.

