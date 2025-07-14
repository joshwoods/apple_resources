

- RealityKit
-  EnvironmentResource 

Class

# EnvironmentResource

An environmental resource that contains background and lighting information for a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class EnvironmentResource
```

## Overview

RealityKit supports image-based lighting that enables realistic reflections on your scene’s 3D content. You can define the look of your scene’s background by supplying an environment resource image that determines the general color of the room, and the location of any spotlights or shadowed areas within the reflection. RealityKit applies the image’s characteristics to your scene’s reflective content.

RealityKit checks a bundle for an environment resource by the filename you supply to one of the load functions.

### Create a skybox folder

To add an environment resource to your Xcode project, make a folder with a name that ends in `.skybox` and place a single image inside. Ensure that the image is an environment map of equirectangular projection, also known as a *latitude-longitude projection*. Drag the folder into the Project navigator. In the options pane, choose to create a folder reference (not a group), and add the folder to your app’s targets. At build time, Xcode compiles the image for use as an environment resource and inserts the result into the app bundle.

RealityKit supports the same input formats as Image I/O, such as `.png` and `.jpg` However, to achieve rich, vibrant lighting, use a `.exr` or `.hdr` format, which support a wide dynamic range.

## Topics

### Loading the resource

convenience init(named: String, in: Bundle?) async throws

Asynchronously loads an environment resource from a bundle.

convenience init(equirectangular: CGImage, withName: String?) throws

Synchronously creates an environment resource from an equirectangular image.

convenience init(equirectangular: CGImage, withName: String?) async throws

Asynchronously generates an environment resource from an equirectangular image.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) async throws

Asynchronously creates an environment resource from a cube texture.

convenience init(cube: TextureResource, options: EnvironmentResource.CreateOptions) throws

Synchronously generates an environment resource from a cube texture resource.

static func load(named: String, in: Bundle?) throws -> EnvironmentResource

Synchronously loads an environment resource from a bundle.

### Configuring the resource creation

struct CreateOptions

A type that controls compression, sampling quality, and cubemap dimensions when creating an environment resource.

typealias Compression

The compression to apply when creating an environment resource.

### Accessing resource data

var skybox: TextureResource

The cube color texture that contains environment surrounding details.

### Deprecated

static func generate(fromEquirectangular: CGImage, withName: String?) throws -> EnvironmentResource

Synchronously generates an environment resource from an equirectangular image.

Deprecated

static func generate(fromEquirectangular: CGImage, withName: String?) async throws -> EnvironmentResource

Asynchronously generates an environment resource from an equirectangular image.

Deprecated

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;EnvironmentResource>

Asynchronously loads an environment resource from a bundle.

Deprecated

## Relationships

### Conforms To

- Resource
- Sendable

## See Also

### Environment

struct EnvironmentLightingConfigurationComponent

A component that scales the amount of light that an entity receives from its environment.

struct VirtualEnvironmentProbeComponent

A component that provides environment lighting for entities you place within the same virtual world.

struct Probe

A sample of the environment around a point in a scene the system uses for environment-based lighting.

enum Source

Options that define the source of diffuse and specular lighting for environment lighting calculations.

