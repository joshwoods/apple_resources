

- RealityKit
-  Combining 2D and 3D views in an immersive app 

Sample Code

# Combining 2D and 3D views in an immersive app

Use attachments to place 2D content relative to 3D content in your visionOS app.

Download

visionOS 2.0+Xcode 16.0+

## Overview

To demonstrate how you can integrate any 2D content into your 3D app, this sample code project uses a variety of frameworks to create both 2D and 3D views, and places them relative to each other in an immersive space. It also illustrates how to position an attachment at the location of a tap gesture.

The rainbow that appears in the sample app contains two USDZ models and four RealityViewAttachments.

- The green arch is a USDZ file from Reality Composer Pro with a custom shader graph material.

- The yellow arch is a USDZ file from Reality Composer Pro with a programmatically created simple material.

- The orange arch is a reality view attachment containing a UIView in a UIViewRepresentable with a custom 2D arc shape.

- The red arch is a reality view attachment containing a `UIView` in a `UIViewRepresentable` with a custom 2D arc shape.

- The pink arch is a reality view attachment containing a SwiftUI View with a custom 2D arc shape.

- The blue arch is a reality view attachment containing a SwiftUI `View` with a custom 2D arc shape.

The app loads the 3D assets from Reality Composer Pro as a ModelEntity in a RealityView, and creates a reality view attachment for each of the 2D arches to attach them to the view.

The cloud attachments at the locations of tap gestures are `RealityViewAttachments` containing Text with an SF Symbols image.

### Load and configure entities from Reality Composer Pro

This sample creates 3D assets in an asset creator and imports them into Reality Composer Pro as `.usdc` files. See Designing RealityKit content with Reality Composer Pro for more information.

The app then configures the appearance of the ModelEntity by setting the material of the ModelComponent, which is the Component that affects appearance. The following code example demonstrates loading a model and configuring the material:

```
```

### Create attachments that contain SwiftUI views

The sample includes the remaining four arches as reality view attachments by creating attachments of various types in the `attachments` closure of a reality view instance. These types include both SwiftUI and UIKit to exemplify how to use any framework in your visionOS app.

```
```

```
```

Attachments can contain views from other frameworks that adopt the `UIViewRepresentable` protocol.

### Add and position entity attachments

The sample loads the attachments as reality view attachments in the `update` closure of the reality view. If there’s an existing attachment for an `id`, the sample adds the attachment entity as a subentity of the plane entity to display it in the scene, and then configures the scale and position.

```
```

This method sets the scales and positions for each attachment by using the yellow arch’s bounding box. This ensures each arch is smaller and further back than the previous. The app applies these scale and position values to each entity in the `update` closure as the code example below shows:

```
```

### Position attachments at the tapped location

Follow these steps to add attachments to RealityKit entities and position them at the tapped location. Ensure that your entities have both an InputTargetComponent and a CollisionComponent.

```
```

Add a SpatialTapGesture to the `RealityView` and make sure it uses targetedToAnyEntity(), or specify which entities to target with targetedToEntity(_:). Then use convert(_:from:to:) to convert the location of the tap gesture from the local coordinate space of the entity to the scene’s coordinate space.

```
```

Create the attachment in the `attachments` closure by iterating over the array of attachments.

```
```

Finally, add each attachment in the `update` closure by iterating over the array of attachments and setting their stored position and root entity.

```
```

## See Also

### Scene content

Hello World

Use windows, volumes, and immersive spaces to teach people about the Earth.

Enabling video reflections in an immersive environment

Create a more immersive experience by adding video reflections in a custom environment.

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Generating interactive geometry with RealityKit

Create an interactive mesh with low-level mesh and low-level texture.

Transforming RealityKit entities using gestures

Build a RealityKit component to support standard visionOS gestures on any entity.

Models and meshes

Display virtual objects in your scene with mesh-based models.

Materials, textures, and shaders

Apply textures to the surface of your scene’s 3D objects to give each object a unique appearance.

Anchors

Lock virtual content to the real world.

Lights and cameras

Control the lighting and point of view for a scene.

Content synchronization

Synchronize the contents of entities locally or across the network.

Audio

Create personalized and realistic spatial audio experiences.

Videos

Present videos in your RealityKit experiences.

