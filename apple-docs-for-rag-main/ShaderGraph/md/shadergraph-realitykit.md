

- ShaderGraph
-  RealityKit 

ShaderGraph Node Group

# RealityKit

Add RealityKit surfaces or textures to your material and access and manipulate scene geometry.

## Overview

Incorporate RealityKit-specific content into your graph and modify that content visually. You can use geometry modifiers to change the vertices of your models. You can also create and configure RealityKit surfaces and textures and use them in your graph.

## Topics

### Nodes

Unlit Surface (RealityKit)

A surface shader that defines properties for a RealityKit Unlit material.

PBR Surface (RealityKit)

A surface shader that defines properties for a RealityKit Physically Based Rendering material.

Occlusion Surface (RealityKit)

A surface shader that defines properties for a RealityKit Occlusion material that does not receive dynamic lighting.

Shadow Receiving Occlusion Surface (RealityKit)

A surface shader that defines properties for a RealityKit Occlusion material that receives dynamic lighting.

View Direction (RealityKit)

A vector from a position in the scene to the view reference point.

Camera Position (RealityKit)

The position of the camera in the scene.

Geometry Modifier Model To World (RealityKit)

The model-to-world transformation Matrix4x4 (Float).

Geometry Modifier World To Model (RealityKit)

The world-to-model transformation Matrix4x4 (Float).

Geometry Modifier Normal To World (RealityKit)

The normal-to-world transformation Matrix3x3 (Float).

Geometry Modifier Model To View (RealityKit)

The model-to-view transformation Matrix4x4 (Float).

Geometry Modifier View To Projection (RealityKit)

The view-to-projection transformation Matrix4x4 (Float).

Geometry Modifier Projection To View (RealityKit)

The projection-to-view transformation Matrix4x4 (Float).

Geometry Modifier Vertex ID (RealityKit)

The integer index of the vertex.

Surface Model To World (RealityKit)

The model-to-world transformation Matrix4x4 (Float).

Surface Model To View (RealityKit)

The model-to-view transformation Matrix4x4 (Float).

Surface World To View (RealityKit)

The world-to-view transformation Matrix4x4 (Float).

Surface View To Projection (RealityKit)

The view-to-projection transformation Matrix4x4 (Float).

Surface Projection To View (RealityKit)

The projection-to-view transformation Matrix4x4 (Float).

Surface Screen Position (RealityKit)

The coordinates of the currently-processed data in screen space.

Surface View Direction (RealityKit)

A vector from a position in the scene to the view reference point.

Environment Radiance (RealityKit)

Returns an environment’s diffuse and specular radiance value based on real-world environment, and an IBL map that is either a developer-provided map or a default map.

Hover State (RealityKit)

Hover State to define custom hover effects

Blurred Background (RealityKit)

Returns a sample of the blurred background.

Geometry Modifier (RealityKit)

A function that manipulates the location of a model’s vertices, run once per vertex.

Camera Index Switch (RealityKit)

Render different results for each eye in a stereoscopic render.

Image 2D (RealityKit)

A texture with RealityKit properties.

Image 2D LOD (RealityKit)

A texture with RealityKit properties and a explicit level of detail.

Image 2D Gradient (RealityKit)

A texture with RealityKit properties and a specified LOD gradient.

Image 2D Pixel (RealityKit)

A texture with RealityKit properties and pixel texture coordinates.

Image 2D LOD Pixel (RealityKit)

A texture with RealityKit properties, a explicit level of detail, and pixel texture coordinates.

Image 2D Gradient Pixel (RealityKit)

A texture with RealityKit properties, a specified LOD gradient, and pixel texture coordinates.

Cube Image (RealityKit)

A texturecube with RealityKit properties.

Cube Image LOD (RealityKit)

A texturecube with RealityKit properties and a explicit level of detail.

Cube Image Gradient (RealityKit)

A texturecube with RealityKit properties and a specified LOD gradient.

Image 2D Read (RealityKit)

Direct texture read.

Image 3D (RealityKit)

A texture with RealityKit properties. Adjustable level of detail.

Image 3D LOD (RealityKit)

A texture with RealityKit properties. Explicit level of detail.

Image 3D Gradient (RealityKit)

A texture with RealityKit properties. Level of detail gradient.

Image 3D Pixel (RealityKit)

A texture with RealityKit properties. Adjustable level of detail. Pixel texture coordinates.

Image 3D LOD Pixel (RealityKit)

A texture with RealityKit properties. Explicit level of detail. Pixel texture coordinates.

Image 3D Gradient Pixel (RealityKit)

A texture with RealityKit properties. Level of detail gradient. Pixel texture coordinates.

Image 2D Array (RealityKit)

A texture with RealityKit properties. Adjustable level of detail.

Image 2D Array LOD (RealityKit)

A texture with RealityKit properties. Explicit level of detail.

Image 2D Array Gradient (RealityKit)

A texture with RealityKit properties. Level of detail gradient.

Image 2D Array Pixel (RealityKit)

A texture with RealityKit properties. Adjustable level of detail. Pixel texture coordinates.

Image 2D Array LOD Pixel (RealityKit)

A texture with RealityKit properties. Explicit level of detail. Pixel texture coordinates.

Image 2D Array Gradient Pixel (RealityKit)

A texture with RealityKit properties. Level of detail gradient. Pixel texture coordinates.

Image 2D Array Read (RealityKit)

Direct texture read.

Image 3D Read (RealityKit)

Direct texture read.

## See Also

### Node Categories

2D-Procedural

Generate 2D gradients, noise, and other patterns programmatically for your material.

2D-Texture

Load and configure 2D texture files.

3D-Procedural

Generate 3D noise patterns programmatically for your material.

3D-Texture

Project multiple 2D images onto a surface to create a 3D texture.

Adjustment

Modify or convert values, or ranges of values, from one form to another.

Application

Get system values such as the current time or the direction of the up vector.

Compositing

Generate a single output from the combination of multiple data values.

Data

Convert data values to different formats, or manipulate individual elements within a data structure.

Geometric

Access scene geometry while your graph runs.

Logic

Perform Boolean operations and other logical comparisons on data values.

Material

Encapsulate a set of shader graph nodes into a single module.

Math

Perform a wide variety of mathematical and transformative operations on data values.

Organization

Modify the visual flow of data within your graph without changing any values.

Procedural

Add a constant number, vector, matrix, color, string, or other value to your graph.

Surface

Generate a MaterialX preview surface.

