

- Core Image
-  Applying a Chroma Key Effect 

Article

# Applying a Chroma Key Effect

Replace a color in one image with the background from another.

## Overview

Use the chroma key effect, also known as bluescreening or greenscreening, to replace the background of an image by setting a color or range of colors to transparent.

Figure 1 Applying a chroma key effect to swap background images

You apply this technique in three steps:

1.  Create a cube map for the colorCube() filter to determine which colors to set transparent.

2.  Apply the `colorCube()` filter to the image to make pixels transparent.

3.  Use the sourceOverCompositing() filter to place the image over the background image.

### Create a Cube Map

A color cube is a 3D color-lookup table that uses the R, G, and B values from the image to lookup a color. To filter out green from the image, create a color map with the green portion set to transparent pixels.

A simple way to construct a color map with these characteristics is to model colors using an HSV (hue-saturation-value) representation. HSV represents hue as an angle around the central axis, as in a color wheel. In order to make a chroma key color from the source image transparent, set its lookup table value to `0` when its hue is in the correct color range.

Figure 2 Color wheel showing the hue values to filter out of a source image with green background

The value for green in the source image falls within the slice beginning at 108° (`108/360` = `0.3`) and ending at 144° (`144/360` = `0.4`). You’ll set transparency to `0` for this range in the color cube.

To create the color cube, iterate across all values of red, green, and blue, entering a value of 0 for combinations that the filter wiill set to transparent. Refer to the numbered list for details on each step to the routine.

1.  Allocate memory. The color cube has three dimensions, each with four elements of data (RGBA).

2.  Use a for-loop to iterate through each color combination of red, green, and blue, simulating a color gradient.

3.  Convert RGB to HSV, as in Listing 2. Even though the color cube exists in RGB color space, it’s easier to isolate and remove color based on hue. Input `0` for green hues to indicate complete removal; use `1` for other hues to leave those colors intact. To specify green as a hue value, convert its angle in the hue pie chart to a range of `0` to `1`. The green in the sample image has hue between `0.3` (`108` out of `360` degrees`)` and `0.4` (`144` out of `360` degrees). Your shade of green may differ, so adjust the range accordingly.

4.  The `colorCube()` filter requires premultiplied alpha values, meaning that the values in the lookup table have their transparency baked into their stored entries rather than applied when accessed.

5.  Create a `colorCube()` filter with the cube data.

Note

The framework doesn’t have built-in direct conversion between color spaces, but you can access the hue of a UIColor created with RGB values. Create a UIColor from the raw RGB values and then read the hue from it.

Listing 2 Converting RGB to HSV

### Remove Green from the Source Image

Apply the color cube filter to a foreground image by setting its `inputImage` parameter and then accessing the `outputImage`.

The output image contains the foreground with all green pixels made transparent.

The filter passes through each pixel in the input image, looks up its color in the color cube, and replaces the source color with the color in the color cube at the nearest position.

### Composite over a Background Image

Chain a `sourceOverCompositing()` filter to the color cube filter to composite a background image to the greenscreened output. The transparency in the colorcube-filtered image allows the composited background image to show through.

The foreground of the source image now appears in front of the background landscape without any trace of the green screen.

## See Also

### Filter Recipes

Selectively Focusing on an Image

Focus on a part of an image by applying Gaussian blur and gradient masks.

Customizing Image Transitions

Transition between images in creative ways using Core Image filters.

Simulating Scratchy Analog Film

Degrade the quality of an image to make it look like dated, analog film.

