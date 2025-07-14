

- UIKit
- UIImage
-  applyingSymbolConfiguration(\_:) 

Instance Method

# applyingSymbolConfiguration(\_:)

Returns a new version of the current image, applying the specified configuration attributes on top of the current attributes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func applyingSymbolConfiguration(_ configuration: UIImage.SymbolConfiguration) -> UIImage?
```

## Parameters 

`configuration`  

The configuration attributes to apply on top of the existing attributes. Values in this object take precedence over the image’s current configuration values.

## Return Value

A new version of the image object that contains the merged configuration details.

## Mentioned in 

Configuring and displaying symbol images in your UI

## Discussion

This method creates a new image object, merging the traits of `configuration` with the new image’s traits. During the merge, this method gives precedence to explicitly set values in the `configuration` parameter. This method then replaces the current image-related attributes with the attributes in `configuration`. If an attribute in `configuration` contains an unspecified value, this method leaves the current image’s setting intact.

## See Also

### Changing the image attributes

func withConfiguration(UIImage.Configuration) -> UIImage

Returns a new version of the current image, replacing the current configuration attributes with the specified attributes.

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

func withBaselineOffset(fromBottom: CGFloat) -> UIImage

Creates a new image with a baseline at the specified offset from the bottom of the image.

class Configuration

A configuration object that contains the traits that the system uses when selecting the current image variant.

class SymbolConfiguration

An object that contains the specific font, size, style, and weight attributes to apply to a symbol image.

