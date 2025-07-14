

- RealityKit
- USD Assets
-  USDZ schemas for AR 

# USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

## Overview

Leveraging Pixar’s Universal Scene Description standard, USDZ delivers AR and 3D content to Apple devices. Apple developed a set of new schemas in collaboration with Pixar to further extend the format for AR use cases. Simply add data to a USDZ file to give your 3D assets AR abilities, such as the ability to:

- Anchor 3D content at a specific location in the real world.

- React to real-world situations.

- Participate in a physics simulation.

- Connect audio effects to a location.

- Annotate the environment by displaying text.

A USDZ file uses these schemas to add features to an augmented reality experience in AR Quick Look or RealityKit in place of `.reality` files`,` `.rcproject` files, or custom code to implement AR functionality. Reality Composer describes AR features in its USDZ export using these schemas, too (see `Exporting a Reality Composer Scene to USDZ`). To enable AR features in assets from a third-party digital content-creation (DCC) tool such as Maya or Houdini, edit the file in `.usda` textual format using the USD Toolset.

Note

These new schemas (see Schema definitions for third-party DCCs) are included in the Universal Scene Description specification as an addendum and are marked as preliminary. The addendum also adds metadata (name-value pairs; see Metadata), and new data properties (Property). To provide feedback on the addendum, use the Feedback Assistant.

### Implement AR functionality

The following illustration depicts a virtual castle rendered by a *runtime*, the app or system framework that implements the AR functionality described in the schemas. The prim for the virtual castle (USD refers to individual units of 3D content as *prims;* see UsdPrim) instructs the runtime to place the castle on a known image in the physical environment, called the image anchor. When the user comes into proximity with the anchor, the runtime displays the 3D visualization of the castle. Falling snowflakes represent additional prims that behave as if in accordance with gravity, and disappear as they approach a real-world surface.

## Topics

### Animation

Control animation playback with metadata.

autoPlay

Metadata that specifies whether an animation plays automatically on load.

playbackMode

Metadata that controls animation idling until a behavior takes over.

### Anchoring

Place a prim at the physical location of a real-world object.

Placing a prim in the real world

Anchor a prim to a real-world object that the runtime recognizes in the physical environment.

Preliminary_AnchoringAPI

A schema that defines the placement of a prim and its children at a real-world location.

Preliminary_ReferenceImage

A schema that defines the properties of an image in the physical environment.

### Behaviors

Actions and triggers

Enable visual and audible responses to programmatic or environmental events.

### Text

Preliminary_Text

A prim that renders 3D text in a scene.

### Scenes and lighting

Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

preferredIblVersion

Metadata that determines the lighting environment of virtual content.

sceneLibrary

Metadata that partitions an asset into scene-based units.

### Digital content creation

Schema definitions for third-party DCCs

Update your local USD library to add interactive and augmented reality features.

## See Also

### Essentials

Exporting a Reality Composer Scene to USDZ

Save a scene or project as USDZ to read, collect, or display in an app or website.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

