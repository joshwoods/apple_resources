

- ShaderGraph
-  Compositing 

ShaderGraph Node Group

# Compositing

Generate a single output from the combination of multiple data values.

## Overview

The compositing process takes multiple input values and combines them in varying proportions to create a single output. You can use Compositing nodes to combine textures and achieve a specific appearance. For example, you might show a background texture only in places where the foreground texture is transparent. Compositing nodes support the combination of colors, but also other data types, such as vectors and floating-point numbers.

## Topics

### Nodes

Premultiply

Multiplies the RGB channels of the input by the alpha channel.

Unpremultiply

Divides the RGB channels of the input by the alpha channel.

Additive Mix

Adds foreground and background values.

Subtractive Mix

Subtracts foreground from background values.

Difference

Outputs the distance between foreground and background values.

Burn

A blend operation that darkens the foreground layer using the background.

Dodge

A blend operation that lightens the background layer depending on the foreground.

Screen

A blend operation that lightens areas that are darker than white.

Overlay

A blend operation that multiplies dark areas and screens light areas.

Disjoint Over

A merge operation that layers foreground over background color, but assumes no overlap in partially transparent areas covered by both.

In

Outputs areas of foreground that overlap with the alpha of background.

Mask

Outputs areas of background that overlap with the alpha of foreground.

Matte

A merge operation that layers premultiplied foreground over background.

Out

Outputs areas of foreground that do not overlap with background.

Over

A merge operation that layers foreground over background, using the alpha of the foreground.

Inside

Multiplies a mask to all channels of the input.

Outside

Multiplies (1 - mask) to all channels of the input.

Mix

Mixes foreground and background inputs, weighting based on mix value.

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

RealityKit

Add RealityKit surfaces or textures to your material and access and manipulate scene geometry.

Surface

Generate a MaterialX preview surface.

