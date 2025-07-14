

- RealityKit
-  Views and attachments 

API Collection

# Views and attachments

Bring RealityKit content into your app with views and renderers.

## Overview

Views are the building blocks for apps that include RealityKit content. Each view displays RealityKit content in your app either by rendering the content in a window, volume, or an immersive space.

## Topics

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewContent

The content of a visionOS reality view.

struct RealityViewCameraContent

The content of a reality view that is displayed through a camera.

protocol RealityViewContentProtocol

A protocol representing the content of a reality view.

struct RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

struct RealityViewEntityCollection

A collection of entities in a RealityView.

protocol EntityCollection

An ordered, mutable collection of entities.

### SwiftUI 3D model presentation

struct Model3D

A view that asynchronously loads and displays a 3D model.

enum Model3DPhase

The current phase of the asynchronous model loading operation.

struct ResolvedModel3D

A view for displaying static three-dimensional models.

struct Model3DPlaceholderContent

A container view that presents either a 3D model or a placeholder for one.

### UIKit and AppKit presentation

class ARView

A view that enables you to display an AR experience with RealityKit.

struct DebugOptions

Options for drawing overlay content in a scene that can aid in debugging.

typealias ARViewBase

The platform-specific base class for the view into which RealityKit renders content.

### Metal workflow rendering

class RealityRenderer

A renderer that displays a RealityKit scene in an existing Metal workflow.

struct CameraSettings

Settings for rendering with a camera.

struct CameraOutput

Output produced by rendering with a camera.

struct ImageBasedLight

Describe the lighting properties for the scene.

struct MetalEventAction

The structure describing an event and value to be signaled or waited for.

struct EntityCollection

A collection of entities in a RealityRenderer.

### SwiftUI view attachments

struct RealityViewAttachmentBuilderContent

A view that gathers the attachment content for your current reality view.

struct Attachment

An attachment content you can use to gather an identifier and view.

struct RealityViewAttachments

The attachments that belong to a RealityView.

class ViewAttachmentEntity

An entity that has a view attachment.

struct ViewAttachmentComponent

A component containing additional information about a view attachment entity provided via the entity(for:) function.

struct TextComponent

A component that draws 2D text at an entity’s location.

### Visual environment adjustments

struct RealityViewEnvironment

A struct that determines the background and default lighting properties for a reality view.

struct RealityViewRenderingEffects

A struct for enabling and disabling rendering effects for RealityKit content.

struct RealityViewRenderingEffectMode

A mode that determines whether a rendering effect is enabled or disabled.

struct RealityViewDynamicRange

Options that determine the state of high dynamic range rendering for virtual content.

enum AntialiasingMode

The rendering technique used to smooth edges of virtual content.

struct Environment

A description of background, lighting, and acoustic properties for a view’s content.

struct RenderOptions

The available rendering options that you use to selectively disable certain rendering effects.

### Postprocessing

Postprocessing effects

Create special rendering effects for your RealityKit scenes.

struct PostProcessContext

An object the framework uses to pass data to a postprocess callback.

struct RenderCallbacks

A container that holds the view’s render callbacks.

### Coordinate space conversions

protocol RealityCoordinateSpaceConverting

A value that can be converted between SwiftUI `CoordinateSpace` and RealityKit `Entity`.

struct SceneRealityCoordinateSpace

The coordinate space that represents the center of a RealityKit scene.

struct CameraRealityCoordinateSpace

The coordinate space that represents the scene’s active camera.

protocol RealityCoordinateSpace

A 3D coordinate space that exists within a RealityKit hierarchy.

protocol RealityCoordinateSpaceProjecting

A protocol for coordinate spaces that can project 2D points to and from 3D.

### Camera mode settings

struct RealityViewCamera

A camera for reality view scenes, that can be world tracking or virtual.

struct CameraControls

enum CameraMode

The available camera modes.

### Attachment types

struct AttachmentContentBuilder

A result builder that creates attachment content from closures.

protocol AttachmentContent

A type that provides content for an attachment content builder.

struct ConditionalAttachmentContent

struct EmptyAttachmentContent

A attachment content that doesn’t contain any content.

struct TupleAttachmentContent

struct AnyAttachmentContent

A type-erased attachment content.

## See Also

### Presentation

Presentation UI

Control your app’s content and how people can interact with it.

