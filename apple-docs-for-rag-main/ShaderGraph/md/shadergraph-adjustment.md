

- ShaderGraph
-  Adjustment 

ShaderGraph Node Group

# Adjustment

Modify or convert values, or ranges of values, from one form to another.

## Overview

Use Adjustment nodes to adjust color values, convert between different color formats, or map input values to a different set of outputs based on rules you specify. For example, you might use these nodes to adapt the output from one node to match the expected input for another node.

## Topics

### Nodes

Remap

Linearly remaps incoming values from one range to another.

Smooth Step

Outputs a smooth remapping from low-high to 0-1.

Luminance

Outputs a grayscale value containing the luminance of the incoming RGB color in all color channels.

RGB to HSV

Converts a color from RGB to HSV space.

HSV to RGB

Converts a color from HSV to RGB space.

Contrast

Increases or decreases contrast of values using a linear slope multiplier.

Range

Remaps incoming values from one range to another.

HSV Adjust

Adjusts the hue, saturation and value of an RGB color by a vector .

Saturate

Adjusts the saturation of a color.

Step (RealityKit)

Outputs a 1 or a 0 depending on whether the input is greater than or less than the edge value.

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

RealityKit

Add RealityKit surfaces or textures to your material and access and manipulate scene geometry.

Surface

Generate a MaterialX preview surface.

