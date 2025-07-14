

- RealityKit
-  ModelComponent 

Structure

# ModelComponent

A component that contains a mesh and materials for the visual appearance of an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct ModelComponent
```

## Mentioned in 

Creating a plane with low-level mesh

## Overview

This component is a foundational component for all visual content in RealityKit. Use `ModelComponent` to render 3D models by attaching it to any Entity in your RealityKit scene.

To create a `ModelComponent`, you need a mesh and the number of materials that mesh expects, which is typically one.

For example, here’s how to create a simple blue, metallic box using generateBox(size:cornerRadius:), and SimpleMaterial:

```
let mesh = MeshResource.generateBox(size: 1, cornerRadius: 0.05)
let material = SimpleMaterial(color: .blue, isMetallic: true)

let modelComponent = ModelComponent(mesh: mesh, materials: [material])

let entity = Entity()
entity.components.set(modelComponent)
```

Make different primitive shapes, like spheres with generateSphere(radius:), or cylinders with generateCylinder(height:radius:), or create custom shapes with MeshDescriptor. For more information about materials, see Applying realistic material and lighting effects to entities

Tip

To load a USDZ or reality file to your app, use an entity initializer such as init(named:in:) or init(contentsOf:withName:).

Use other components like CollisionComponent, PhysicsBodyComponent, PhysicsMotionComponent, and InputTargetComponent to make entities interactive and dynamic.

## Topics

### Creating a model component

init(mesh: MeshResource, materials: [any Material])

Creates a model component from a mesh and a collection of materials.

### Configuring a mesh

var mesh: MeshResource

The mesh that defines the model’s shape.

### Configuring the materials

var materials: [any Material]

The materials that define the model’s visual appearance.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Modifying the bounding box for rendering

var boundsMargin: Float

A margin applied to an entity’s bounding box that determines object visibility.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Model display

class MeshResource

A high-level representation of a collection of vertices and edges that define a shape.

class ModelEntity

A representation of a physical object that RealityKit renders and optionally simulates.

