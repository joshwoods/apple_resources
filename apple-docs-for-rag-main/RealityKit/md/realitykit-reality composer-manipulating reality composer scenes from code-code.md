

- RealityKit
- Reality Composer
-  Manipulating Reality Composer scenes from code 

Article

# Manipulating Reality Composer scenes from code

Make programmatic changes to your scenes at runtime.

## Overview

Although *Reality Composer* behaviors provide a way to add interactivity to your scene without writing code, there are times when the only way to implement functionality is to make changes from code. You can manipulate the objects in your scene in many different ways, including hiding or duplicating them, or changing their location, orientation, and scale.

### Access scene objects

To retrieve specific objects from a scene, first assign each object a name in Reality Composer, using the Properties inspector. If you give an object a unique name, Xcode automatically creates an accessor property during code generation. For example, if you have an object called Steel Box in a scene named Box that’s contained in a file called `Experience.reality`, you can get a reference to that object by using code like this:

```
if let boxScene = try? Experience.loadBox() {
    let box = boxScene.steelBox
    // Do something with box.
}
```

If you give multiple objects in a scene the same name, the generated property returns an array containing all of the objects that share that name.

If you need to load a named object without using generated code, such as when working with downloaded reality files or loading objects created at runtime, you can use the findEntity(named:) function on the scene entity.

```
if let boxScene = try? Experience.loadBox() {
    if let box = boxScene.findEntity(named: "Steel Box") {}
        // Do something with box
    }
}
```

### Hide and show entities

In addition to hiding and showing objects in your scene using behaviors, as described in Bringing a Reality Composer scene to life, you can also use code to hide and show them, by using the isEnabled property. If you set an object’s isEnabled property to false, ARKit doesn’t render it and it doesn’t participate in the scene’s physics simulation. If you set it back to true, ARKit starts rendering the object again and it resumes participating in the physics simulation.

Note

Child objects of the isEnabled property inherit its settings, so disabling isEnabled also disables all of its children.

### Transform a scene object

You can transform (move, rotate, or scale) objects in a scene by using the transform property of the Entity.

To move an object, change the translation value of the transform. For example, to move a scene object 10 cm along the x-axis, use this:

```
myEntity.transform.translation += SIMD3(10, 0, 0)
```

Similarly, to scale an object, modify the scale of the entity’s transform property. For example, you can double the size of an object in your scene like this:

```
myEntity.transform.scale *= 2
```

To rotate an object, make changes to the rotation property of its transform. This code shows you how to rotate an object in your scene by 90° on the z-axis:

```
// Calculate 90° as radians.
let radians = 90.0 * Float.pi / 180.0

// Create a quaternion that represents a 90° rotation on the z-axis
// and add it to the existing rotation value.
anchorEntity.transform.rotation += simd_quatf(angle: radians, 
                                              axis: SIMD3(0,0,1))
```

### Clone an entity

If you need to create multiple copies of the same object at runtime, avoid loading the entity multiple times, which can cause performance issues. Instead, load a single copy of the entity before you need it, but don’t add it to your scene. When you need a new instance, call the clone(recursive:) function on the loaded entity, and then add the clone as a child of a scene anchor.

Here’s an example of cloning an anchored entity and adding it to your ARView:

```
let copy = myEntity.clone(recursive: true)
```

### Add force to an object

If an object in a scene participates in the physics simulation, you can add force to that object from code by using the addForce(_:relativeTo:) method. Provide a vector representing the amount and direction of force to add to the object as the first parameter. Here’s an example of applying force to an object to make it fly away from the camera:

```
// Adjusting the forceMultiplier value changes the amount of force applied.
let forceMultiplier = simd_float3(repeating: 10)
ball.addForce(simd_float3(x: cameraForwardVector.x,
                          y: cameraForwardVector.y,
                          z: cameraForwardVector.z) * forceMultiplier,
              relativeTo: nil)
```

## See Also

### Scene creation

Creating 3D Content with Reality Composer

Assemble assets into a dynamic 3D composition that you can add to a scene in your app, or share with AR Quick Look.

Loading Reality Composer files using generated code

Leverage automatically generated code to load scenes from Xcode.

Loading Reality Composer files manually without generated code

Load Reality Composer files that aren’t part of your Xcode project.

Adding elements to a 3D scene

Add assets to your scene from Reality Composer’s library, or import custom assets.

Configuring elements in a scene

Define the appearance and behavior of objects in a scene.

Arranging elements in a scene

Manipulate objects to complete your Reality Composer scene.

Adding procedural assets to a scene

Create procedurally generated shape primitives to your Reality Composer scene.

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

