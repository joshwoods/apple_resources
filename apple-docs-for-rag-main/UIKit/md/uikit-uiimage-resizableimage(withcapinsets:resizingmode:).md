

- UIKit
- UIImage
-  resizableImage(withCapInsets:resizingMode:) 

Instance Method

# resizableImage(withCapInsets:resizingMode:)

Returns a new version of the image with the specified cap insets and options.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func resizableImage(
    withCapInsets capInsets: UIEdgeInsets,
    resizingMode: UIImage.ResizingMode
) -> UIImage
```

## Parameters 

`capInsets`  

The values to use for the cap insets.

`resizingMode`  

The mode with which the interior of the image is resized.

## Return Value

A new image object with the specified cap insets and resizing mode.

## Discussion

This method is exactly the same as its counterpart resizableImage(withCapInsets:) except that the resizing mode of the new image object can be explicitly declared. You should only call this method in place of its counterpart if you specifically want your image to be resized with the UIImage.ResizingMode.stretch resizing mode.

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

func resizableImage(withCapInsets: UIEdgeInsets) -> UIImage

Returns a new version of the image with the specified cap insets.

func imageWithoutBaseline() -> UIImage

Creates a copy of the current image object without any baseline information.

func withBaselineOffset(fromBottom: CGFloat) -> UIImage

Creates a new image with a baseline at the specified offset from the bottom of the image.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

