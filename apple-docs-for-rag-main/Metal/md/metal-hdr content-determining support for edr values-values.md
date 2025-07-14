

- Metal
- HDR Content
-  Determining Support for EDR Values 

Article

# Determining Support for EDR Values

Check whether a display supports EDR.

## Overview

To find out whether a display can support EDR values, read the maximumPotentialExtendedDynamicRangeColorComponentValue property on an NSScreen object for that display. A value greater than 1.0 indicates that the display supports EDR values; otherwise, the display supports only SDR values.

This property’s value is independent of the current state of the display. It’s possible for a display to support EDR but to be unable to present those values right now. For information about the current state of the display, check the maximumExtendedDynamicRangeColorComponentValue property.

## See Also

### High Dynamic Range Content

Processing HDR Images with Metal

Implement a post-processing pipeline using the latest features on Apple GPUs.

Displaying HDR Content in a Metal Layer

Bring your high dynamic range (HDR) content to compatible Mac displays.

Using Color Spaces to Display HDR Content

Use a color space when you don’t need to edit or process the pixel data.

Using System Tone Mapping on Video Content

Use EDR metadata to apply the default system tone mapping to a layer.

Performing Your Own Tone Mapping

Apply your own tone mapping to get the exact behavior you want.

Implementing Tone Mapping on Reference Displays

Detect reference displays and keep your content within the capabilities of the display hardware.

