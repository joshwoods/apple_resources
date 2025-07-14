

- Foundation
- NSString
-  draw(with:options:attributes:context:) 

Instance Method

# draw(with:options:attributes:context:)

Draws the attributed string in the specified bounding rectangle using the provided options.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**macOS**

``` source
func draw(
    with rect: CGRect,
    options: NSString.DrawingOptions = [],
    attributes: [NSAttributedString.Key : Any]? = nil,
    context: NSStringDrawingContext?
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func draw(
    with rect: CGRect,
    options: NSStringDrawingOptions = [],
    attributes: [NSAttributedString.Key : Any]? = nil,
    context: NSStringDrawingContext?
)
```

## Parameters 

`rect`  

The bounding rectangle in which to draw the string.

`options`  

Additional drawing options to apply to the string during rendering. For a list of possible values, see NSStringDrawingOptions.

`attributes`  

The text attributes with which to draw the string. These are the same attributes that can be applied to an `NSAttributedString` object, but in the case of `NSString` objects, the attributes apply to the entire string, rather than ranges within the string.

`context`  

A context object with information about how to adjust the font tracking and scaling information. On return, the specified object contains information about the actual values used to render the string. This parameter may be `nil`.

## Discussion

This method draws as much of the string as it can inside the specified rectangle, wrapping the string text as needed to make it fit. If the string is too big to fit completely inside the rectangle, the method scales the font or adjusts the letter spacing to make the string fit within the given bounds.

If newline characters are present in the string, those characters are honored and cause subsequent text to be placed on the next line underneath the starting point. To correctly draw and size multi-line text, pass usesLineFragmentOrigin in the options parameter.

### Special Considerations

This method uses the baseline origin by default.

If usesLineFragmentOrigin is not specified, the rectangle’s height will be ignored and the operation considered to be single-line rendering.

## See Also

### Sizing and Drawing Strings

func draw(at: CGPoint, withAttributes: [NSAttributedString.Key : Any]?)

Draws the receiver with the font and other display characteristics of the given attributes, at the specified point in the current graphics context.

func draw(in: CGRect, withAttributes: [NSAttributedString.Key : Any]?)

Draws the attributed string inside the specified bounding rectangle.

func boundingRect(with: CGSize, options: NSStringDrawingOptions, attributes: [NSAttributedString.Key : Any]?, context: NSStringDrawingContext?) -> CGRect

Calculates and returns the bounding rect for the receiver drawn using the given options and display characteristics, within the specified rectangle in the current graphics context.

func size(withAttributes: [NSAttributedString.Key : Any]?) -> CGSize

Returns the bounding box size the receiver occupies when drawn with the given attributes.

func variantFittingPresentationWidth(Int) -> String

Returns a string variation suitable for the specified presentation width.

struct NSStringDrawingOptions

Constants that specify the rendering options for drawing a string.

