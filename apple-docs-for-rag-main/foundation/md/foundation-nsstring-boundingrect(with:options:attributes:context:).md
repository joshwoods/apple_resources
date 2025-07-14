

- Foundation
- NSString
-  boundingRect(with:options:attributes:context:) 

Instance Method

# boundingRect(with:options:attributes:context:)

Calculates and returns the bounding rect for the receiver drawn using the given options and display characteristics, within the specified rectangle in the current graphics context.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func boundingRect(
    with size: CGSize,
    options: NSStringDrawingOptions = [],
    attributes: [NSAttributedString.Key : Any]? = nil,
    context: NSStringDrawingContext?
) -> CGRect
```

**macOS**

``` source
func boundingRect(
    with size: CGSize,
    options: NSString.DrawingOptions = [],
    attributes: [NSAttributedString.Key : Any]? = nil,
    context: NSStringDrawingContext?
) -> CGRect
```

## Parameters 

`size`  

The size of the rectangle to draw in.

`options`  

String drawing options.

`attributes`  

A dictionary of text attributes to be applied to the string. These are the same attributes that can be applied to an `NSAttributedString` object, but in the case of `NSString` objects, the attributes apply to the entire string, rather than ranges within the string.

`context`  

The string drawing context to use for the receiver, specifying minimum scale factor and tracking adjustments.

## Return Value

The bounding rect for the receiver drawn using the given options and display characteristics. The rect origin returned from this method is the first glyph origin.

## Discussion

To correctly draw and size multi-line text, pass usesLineFragmentOrigin in the options parameter.

This method returns fractional sizes (in the `size` component of the returned CGRect); to use a returned size to size views, you must raise its value to the nearest higher integer using the ceil function.

This method returns the actual bounds of the glyphs in the string. Some of the glyphs (spaces, for example) are allowed to overlap the layout constraints specified by the size passed in, so in some cases the width value of the size component of the returned CGRect can exceed the width value of the `size` parameter.

## See Also

### Sizing and Drawing Strings

func draw(at: CGPoint, withAttributes: [NSAttributedString.Key : Any]?)

Draws the receiver with the font and other display characteristics of the given attributes, at the specified point in the current graphics context.

func draw(in: CGRect, withAttributes: [NSAttributedString.Key : Any]?)

Draws the attributed string inside the specified bounding rectangle.

func draw(with: CGRect, options: NSStringDrawingOptions, attributes: [NSAttributedString.Key : Any]?, context: NSStringDrawingContext?)

Draws the attributed string in the specified bounding rectangle using the provided options.

func size(withAttributes: [NSAttributedString.Key : Any]?) -> CGSize

Returns the bounding box size the receiver occupies when drawn with the given attributes.

func variantFittingPresentationWidth(Int) -> String

Returns a string variation suitable for the specified presentation width.

struct NSStringDrawingOptions

Constants that specify the rendering options for drawing a string.

