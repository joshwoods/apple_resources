

- UIKit
- UIImage
-  withAlignmentRectInsets(\_:) 

Instance Method

# withAlignmentRectInsets(\_:)

Returns a new version of the image that uses the specified alignment insets.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func withAlignmentRectInsets(_ alignmentInsets: UIEdgeInsets) -> UIImage
```

## Parameters 

`alignmentInsets`  

The alignment metadata to apply to the new image.

## Return Value

A new image object.

## See Also

### Related Documentation

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

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

func resizableImage(withCapInsets: UIEdgeInsets) -> UIImage

Returns a new version of the image with the specified cap insets.

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

