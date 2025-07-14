

- Xcode
- Debugging
- Metal debugger
-  Inspecting textures 

Article

# Inspecting textures

Discover issues in your textures by examining their content.

## Overview

The Metal debugger allows you to view the contents of a texture in the Texture viewer. First, flip the texture to the correct orientation and adjust the colors to ensure accuracy. Then, check for pixel issues like infinite values, not-a-number values, or any values that exceed the current EDR headroom of your display. Hover over pixels within the texture to inspect their values, then find any anomalies by selecting a pixel and comparing it with others. Finally, compare across mipmap levels to check for visual issues. For more information, see Inspecting the bound resources for a command or Analyzing memory usage.

### Navigate your texture

The Texture viewer contains several controls for interacting with and displaying your texture. If your texture contains multiple slices, such as MTLTextureType.type2DArray, the controls in the title bar are disabled until you click a texture image. The active texture image has a system accent color border.

Groups of texture slices that contain related content, such as the faces for a texture of type MTLTextureType.typeCube, are part of the same texture image.

### Flip your texture

If your renderer is using a different coordinate system and your texture image is upside down or flipped horizontally, you can flip it to the correct orientation in the Texture viewer. Click the texture actions button, then choose Flip Horizontally or Flip Vertically. Xcode flips groups of related texture slices, such as cubemaps, as a whole, and it flips unrelated texture slices independently.

### Configure texture rendering

Xcode automatically configures the color properties based on your texture, but you can configure them manually by clicking the Colors button in the title bar. You configure texture rendering on a per-texture-image basis. Follow these guidelines:

- Set the color space to the one that the device display uses. For example, use sRGB if you’re debugging an iPhone workload.

- If you’re using a display that supports extended dynamic range, you can enable the Extended Dynamic Range Content option to render the texture with extended range. When this option is enabled, Xcode draws hatching on any pixels containing values above your display EDR headroom. Consider lowering the brightness of your display to increase the available headroom.

- Xcode shows additional controls to manually configure rendering if you select Default (No color-match) as the color space. You can then configure the range of visible colors, channel swizzling, and whether the alpha is premultiplied.

### View texture properties

You can view properties for the active texture image, such as width and height, by clicking the Info button in the title bar.

### View texture issues

The Issues button in the title bar becomes active if your texture contains any pixels (or samples) with values that are infinite, are not-a-number, or exceed the current EDR headroom of your display.

You can click the Issues button to see more information, and then click the Jump button to focus on a pixel (or sample) causing the issue.

### Inspect, select, and compare pixel values

Move the pointer over a pixel (or a sample if your texture is of type MTLTextureType.type2DMultisample or MTLTextureType.type2DMultisampleArray) to inspect its value.

Then, you can select the pixel by clicking it. Alternatively, you can click and hold so that Xcode selects the pixel, zooms in, and immediately opens the value inspector.

You can also select a pixel using the coordinate input controls on the right of the control bar. Type in the coordinates for the pixel you want, such as `X: 100` and `Y: 100`. Depending on your texture configuration, Xcode may show additional controls.

Click the Jump button in the control bar to zoom in to the selected pixel or sample. Xcode automatically focuses when you click the stepper to the right of each text field.

You can also move the pointer over a different pixel (or sample) to compare the values. If the selected pixel is to the left of the pixel beneath the pointer, the values of the selected pixel appear on the left of the inspector. If it’s to the right, the values appear on the right. Xcode highlights the coordinates for the selected pixel in the inspector to show which values correspond to which pixel.

If you open multiple Attachments viewers or Texture viewers, you can compare pixels across different textures. For information on configuring editors within your Xcode workspace, see Configuring the Xcode project window.

### Compare mipmap levels

By default, the Texture viewer shows all of your texture’s mipmap levels side by side. However, if you want to visually compare different mipmap levels, you can enable stacking. Click the texture actions button, and then choose Stack Mips.

Drag the slice slider in the control bar to visually compare different mipmap levels.

Note

By default, the Texture viewer stacks 3D textures, such as MTLTextureType.type3D, using the z-coordinate. You can disable stacking to see the depth slices side by side. If your 3D texture has multiple mipmap levels, you can choose either Stack Mips or Stack Z.

## See Also

### Metal resource inspection

Inspecting acceleration structures

Reveal ray intersection bottlenecks by examining your acceleration structures.

Inspecting buffers

Confirm your buffer formats by examining buffer content.

Inspecting pipeline states

Determine how your render and compute passes behave by examining their properties.

Inspecting sampler states

Verify your sampler state configurations by examining their properties.

Inspecting shaders

Improve your app’s shader performance by examining and editing your shaders.

