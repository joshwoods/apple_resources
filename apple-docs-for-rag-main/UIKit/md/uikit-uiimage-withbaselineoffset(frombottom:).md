

- UIKit
- UIImage
-  withBaselineOffset(fromBottom:) 

Instance Method

# withBaselineOffset(fromBottom:)

Creates a new image with a baseline at the specified offset from the bottom of the image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withBaselineOffset(fromBottom baselineOffset: CGFloat) -> UIImage
```

## Parameters 

`baselineOffset`  

The position of the baseline, relative to the bottom of the image. Specify this value in points, where positive values move the baseline up from the bottom of the image and negative values move the baseline down.

## Return Value

A new image object containing the baseline information.

## Mentioned in 

Configuring and displaying symbol images in your UI

## Discussion

Use this method to create an image with the specified baseline information. You might add a baseline to your custom images so that you can incorporate them into text-based layouts. You can also use this method to change the baseline information on an image.

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

func resizableImage(withCapInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode) -> UIImage

Returns a new version of the image with the specified cap insets and options.

func imageWithoutBaseline() -> UIImage

Creates a copy of the current image object without any baseline information.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

