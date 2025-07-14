

- RealityKit
- Entity
-  Creating USD files for Apple devices 

# Creating USD files for Apple devices

Generate 3D assets that render as expected.

## Overview

Universal Scene Description (USD) is a comprehensive 3D content-creation technology that supports a variety of real-time and offline workflows. Depending on the device and its operating system, there are three renderers that might display a 3D asset you create for your real-time apps and AR experiences: RealityKit, SceneKit, or Storm. Each renderer supports a specific subset of the USD features. Use only USD features supported by the renderer that displays your asset to ensure that it renders and functions as desired. For detailed information about which USD features each renderer supports, see Validating Feature Support for USD Files.

All three renderers use a physically based rendering (PBR) technique that the USD specification calls the *metallic workflow*. A metallic workflow shader takes metallic, roughness, and base color values as its core inputs. Most digital content-creation tools (DCCs) support PBR metallic workflow shaders and many of them default to using it.

USD and many DCCs also support a second PBR technique called the *specular workflow* (sometimes also called the *glossy workflow*). The specular workflow renders assets by using another algorithm that takes different input values. Only Storm supports the specular workflow, so for maximum compatibility, use metallic workflow shaders in your DCC, or your preview renders won’t accurately represent how your final rendered asset looks.

Note

Find more information and an example shader implementation for both of USD’s PBR workflows by reading the USDPreviewSurface shader page in the USD specification.

## Target a renderer

Your app’s operating system will use one of three renderers, based on these factors:

RealityKit  
The RealityKit renderer is part of the RealityKit framework. It handles drawing for Reality Composer, Reality Composer Pro and RealityKit scenes. QuickLook uses RealityKit to render USDZ files.

SceneKit  
The SceneKit renderer is part of the SceneKit framework. It renders 3D content in Xcode, Motion, and all other apps that use the SceneKit framework.

Storm  
The Storm renderer is a Metal-native implementation of Pixar’s high-performance preview renderer. Quicklook on macOS uses Storm to render USD, USDA and USDC files. Preview on macOS also uses Storm to display all USD file types.

Use the process outlined below to ensure that your USD assets render correctly and function as expected in your app.

## Validate your USD assets

USD files that aren’t well-formed may not work correctly. Validate that your assets conform to the USD specification before including them in your app by using OpenUSD’s `usdchecker` command-line tool with the `--arkit` flag. The `usdchecker` command-line tool is available with macOS starting with macOS 15.

## Use the latest USD schemas

The USD adoption process often results in changes to proposed schemas before they become part of the specification. If you’ve created any assets using a preliminary schema, re-export them using the standard USD schema once the features your asset uses become part of the specification.

Note

Only the RealityKit renderer supports custom preliminary schemas.

## Target your use of subdivision

USD supports a feature called *subdivision surfaces*, which tells the renderer to generate additional geometry on-the-fly to make the entity render more smoothly. Target your use of this feature to instances when you most need smooth rendering. Each level of subdivision increases the number of rendered polygons in the model by a factor of four, which can have substantial performance implications.

Note

The default `subdivisionScheme` value in USD is `catmullClark`, a subdivision surfaces algorithm. This means subdivision surfaces is automatically enabled for assets that don’t explicitly include a subdivision scheme. To ensure that subdivision surfaces is not enabled for your asset, explicitly set `subdivisionScheme` to `none` when exporting from a DCC. For more information, see the documentation for GetSubdivisionSchemeAttr() in the USD specification. You can also use the support scripts below to set `subdivisionScheme` to `none` automatically in your USD files.

## Target your use of double sided geometry

USD geometry can be set to render both sides of a surface by setting the `doubleSided` attribute. Target your use of this feature as its support varies by renderer, which may affect how your content is represented, and its performance.

Note

The default `doubleSided` value is off, however some DCCs enable it automatically during export. It is recommended to review your applications export settings to make sure it is only enabled when desired. You can also use the support scripts below to turn off `doubleSided` on your geometry.

## Limit rigged models to a single skeleton

USD supports skeletal animation, which you can use to animate a character or other complex model by manipulating a hierarchy of bones or joints to deform the model. Many DCCs allow you to use multiple *skeletons* (sometimes called *armatures* or *rigs*), to deform a single mesh. For example, for a character model, you might create one skeleton to handle facial animation and a second one to control general body movement. Before exporting models with multiple skeletons to a USD file, merge all the skeletons into a single joint or bone hierarchy. Models with multiple hierarchies can cause performance and compatibility issues with all three renderers.

Note

All DCCs implement skeletal animation using either a hierarchy of bones or joints. Both approaches deform the model for animation, but use different underlying data representations. DCCs that use bone-based skeletons automatically convert the skeleton to joints when exporting to USD, because USD only supports joint-based skeletons.

## Include material and skeleton bindings

USD requires that any geometry with an applied material use the `MaterialBindingAPI`. It also requires that any geometry that has a skeleton use the `SkelBindingAPI`. Without these APIs, the material or skeleton information may not be read by an application.

Note

Some DCC versions may not correctly apply these bindings in a USD. You can use the support script below to automatically apply them to geometry that has the attributes.

## Expose configurations as variants

USD supports the ability to have multiple representations of an object using a feature called `variants`. USD files define the primary hierarchy path in the file using the `defaultPrim` metadata. Variants that are defined this `defaultPrim` hierarchy path are shown to the user as configuration options when using QuickLook with USDZ files. The variant configuration interface is available starting with visionOS 2, macOS 15, iOS 18 and iPadOS 18. When a configuration option is selected, the appearance of the USD being viewed in QuickLook will change to respect the selected variant.

Note

Variants can be authored in some DCCs or using the USD API. You can also use the support script below to combine USDZ files into a single file as variants, as long as they only vary in their material or skeleton animations.

## Support scripts

We provide a set of scripts to assist you in creating great USD files, using the OpenUSD Python API. These scripts will help address many of the points above within your USD files, or enable you to create USDZ files using variants.

To download these scripts, see USD Support Scripts.

## Topics

### Validating USD feature support

Validating feature support for USD files

Ensure that the renderer that displays your USD assets supports its features.

## See Also

### Loading an entity from a file

Loading entities from a file

Retrieve an entity from storage on disk using a synchronous or an asynchronous load operation.

Stored entities

Manage entities that you store as assets on disk.

convenience init(contentsOf: URL, withName: String?) async throws

Creates an entity by asynchronously loading it from a file URL.

convenience init(named: String, in: Bundle?) async throws

Creates an entity by asynchronously loading it from a bundle.

struct ReferenceComponent

A component that can load another entity from a file.

