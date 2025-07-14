

- Foundation
- NSString
-  size(withAttributes:) 

Instance Method

# size(withAttributes:)

Returns the bounding box size the receiver occupies when drawn with the given attributes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func size(withAttributes attrs: [NSAttributedString.Key : Any]? = nil) -> CGSize
```

## Parameters 

`attrs`  

A dictionary of text attributes to be applied to the string. These are the same attributes that can be applied to an `NSAttributedString` object, but in the case of `NSString` objects, the attributes apply to the entire string, rather than ranges within the string.

## Return Value

The bounding box size the receiver occupies when drawn with the specified attributes.

## Discussion

This method returns fractional sizes; to use a returned size to size views, you must raise its value to the nearest higher integer using the ceil function.

## See Also

### Sizing and Drawing Strings

func draw(at: CGPoint, withAttributes: [NSAttributedString.Key : Any]?)

Draws the receiver with the font and other display characteristics of the given attributes, at the specified point in the current graphics context.

func draw(in: CGRect, withAttributes: [NSAttributedString.Key : Any]?)

Draws the attributed string inside the specified bounding rectangle.

func draw(with: CGRect, options: NSStringDrawingOptions, attributes: [NSAttributedString.Key : Any]?, context: NSStringDrawingContext?)

Draws the attributed string in the specified bounding rectangle using the provided options.

func boundingRect(with: CGSize, options: NSStringDrawingOptions, attributes: [NSAttributedString.Key : Any]?, context: NSStringDrawingContext?) -> CGRect

Calculates and returns the bounding rect for the receiver drawn using the given options and display characteristics, within the specified rectangle in the current graphics context.

func variantFittingPresentationWidth(Int) -> String

Returns a string variation suitable for the specified presentation width.

struct NSStringDrawingOptions

Constants that specify the rendering options for drawing a string.

