

- UIKit
- UIImage
-  resizableImage(withCapInsets:) 

Instance Method

# resizableImage(withCapInsets:)

Returns a new version of the image with the specified cap insets.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func resizableImage(withCapInsets capInsets: UIEdgeInsets) -> UIImage
```

## Parameters 

`capInsets`  

The values to use for the cap insets.

## Return Value

A new image object with the specified cap insets.

## Discussion

You use this method to add cap insets to an image or to change the existing cap insets of an image. In both cases, you get back a new image and the original image remains untouched. For example, you can use this method to create a background image for a button with borders and corners: when the button is resized, the corners of the image remain unchanged, but the borders and center of the image expand to cover the new size.

iOS uses different rendering techniques, with different performance characteristics, depending on the size of each resizable area in the image:

- If resizable areas have a width or height of 1 pixel—that is, a horizontally resizable area is 1 pixel wide, a vertically resizable area is 1 pixel tall, or the center region of the image is 1 x 1 pixel—iOS draws the image by stretching the 1-pixel region. This mode provides the fastest performance (for nonzero cap insets).

- If resizable areas have a width or height greater than 1 pixel, iOS draws the image by tiling the region. This mode provides reduced performance, but can be useful for images with textured (rather than solid-color) content in their resizable areas.

- If the entire image is resizable—that is, the `capInsets` parameter is zero—and its size is greater than 1 x 1 pixel, iOS draws the image by tiling the entire image. This mode is faster than the tiling mode for nonzero cap insets.

To instead directly control the resizing mode, use the resizableImage(withCapInsets:resizingMode:) method.

## See Also

### Changing the image attributes

func withConfiguration(UIImage.Configuration) -> UIImage

Returns a new version of the current image, replacing the current configuration attributes with the specified attributes.

func applyingSymbolConfiguration(UIImage.SymbolConfiguration) -> UIImage?

Returns a new version of the current image, applying the specified configuration attributes on top of the current attributes.

func imageFlippedForRightToLeftLayoutDirection() -> UIImage

Returns a new version of the current image that flips horizontally when it’s in a right-to-left layout.

func withHorizontallyFlippedOrientation() -> UIImage

Returns a new version of the image that’s a mirror of the original image.

func withRenderingMode(UIImage.RenderingMode) -> UIImage

Returns a new version of the image that uses the specified rendering mode.

func withAlignmentRectInsets(UIEdgeInsets) -> UIImage

Returns a new version of the image that uses the specified alignment insets.

func resizableImage(withCapInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode) -> UIImage

Returns a new version of the image with the specified cap insets and options.

func imageWithoutBaseline() -> UIImage

Creates a copy of the current image object without any baseline information.

func withBaselineOffset(fromBottom: CGFloat) -> UIImage

Creates a new image with a baseline at the specified offset from the bottom of the image.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

