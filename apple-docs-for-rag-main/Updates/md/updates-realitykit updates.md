

- Updates
-  RealityKit updates 

Article

# RealityKit updates

Learn about important changes in RealityKit.

## Overview

Browse notable changes in RealityKit.

## June 2024

### General

- Add artistic lights and shadows to your visionOS app with PointLightComponent, DirectionalLightComponent, SpotLightComponent, and DynamicLightShadowComponent.

- Manage spatial tracking in your app with the SpatialTrackingSession.

- Use LowLevelMesh to efficiently bring your mesh data to RealityKit, including custom vertex attributes, formats, and layouts.

- Use an AnimationLibraryComponent to store associated animations with an entity that plays the animations.

- Create an IKComponent to animate a skeletal model with an inverse kinematics IKComponent.Solver.

- Use an AudioLibraryComponent to store associated audio with an entity that plays the audio.

- Stream generated audio in real time with AudioGeneratorController.

- Manage the meshes on your blend shapes with BlendShapeWeightsComponent.

- Create more engaging sound effects by configuring rolloff and reverb with the SpatialAudioComponent.

- Customize hover effects when using HoverEffectComponent, such as spotlight styles, highlight styles, or shader-backed hover effects for additional control over hover behaviors.

- Create an environment resource from a cube texture that has quality and compression options with doc://com.apple.documentation/documentation/realitykit/environmentresource/init(cube:options:)-5v70i, and access environment resources with skybox.

### Models and materials

- Optimize material initialization with a CustomMaterial.Program to compile backing shaders.

- Bring your two-dimensional vector content into 3D with doc://com.apple.documentation/documentation/realitykit/meshresource/init(extruding:extrusionoptions:)-3h21u.

- Control the compression of loaded textures with compression.

- Create texture resources from doc://com.apple.documentation/documentation/realitykit/textureresource/cubemap(slices:named:options:)-7k9y6, texture2DArray(slices:named:options:) or texture3D(slices:named:options:).

- Use init(from:) to efficiently update custom texture data in RealityKit, including custom pixel formats, texture types, swizzle, and texture usage.

- Create cube texture resources with init(cubeFromEquirectangular:named:quality:faceSize:options:) or init(cubeFromImage:named:options:).

- Create cube, 2D array, and 3D texture resources from data with doc://com.apple.documentation/documentation/realitykit/textureresource/init(dimensions:format:contents:)-28vgd, init(dimensions:format:contents:), or init(dimensions:format:contents:).

- Access additional texture resource properties: arrayLength, depth, pixelFormat, and textureType.

- Add a clearcoat to your custom materials with clearcoatNormal.

### Physics and simulations

- Apply force effects on rigid bodies with the ForceEffect.

- Create simulations such as hinge and slider joints with PhysicsJoint.

### Immersive environments

- Anchor dockable videos by attaching a DockingRegionComponent to your entity.

- Peer into other immersive worlds with a PortalComponent, and allow objects from that world to enter yours with PortalCrossingComponent.

- Further control the lighting in your environment with EnvironmentLightingConfigurationComponent.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

