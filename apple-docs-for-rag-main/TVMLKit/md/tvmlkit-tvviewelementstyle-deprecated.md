

- TVMLKit
-  TVViewElementStyle Deprecated

Class

# TVViewElementStyle

A style applied to a view element.

tvOS 9.0–18.0Deprecated

``` source
class TVViewElementStyle
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Retrieving the Style for an Element

func value(propertyName: String) -> Any?

Returns the value associated with a given style name.

### Defining the Height and Width of an Element

var height: CGFloat

The height, in pixels, for an element.

var maxHeight: CGFloat

The maximum height, in pixels, for the element.

var maxWidth: CGFloat

The maximum width, in pixels, for an element.

var minHeight: CGFloat

The minimum height, in pixels, for an element.

var minWidth: CGFloat

The minimum width, in pixels, for an element.

var width: CGFloat

The width, in pixels, for an element.

### Aligning and Positioning an Element

var alignment: TVElementAlignment

A value indicating how an item is aligned inside of an element.

enum TVElementAlignment

Location of an item inside of an element on the horizontal axis.

var contentAlignment: TVElementContentAlignment

A value indicating how items inside of an element are aligned.

enum TVElementContentAlignment

Location of items inside of an element on the vertical axis.

var focusMargin: UIEdgeInsets

The amount of space, in pixels, a custom cell requires when it comes into focus.

var interitemSpacing: CGFloat

The spacing, in pixels, between items inside of an element.

var margin: UIEdgeInsets

The amount of space, in pixels, between the element and other elements.

var padding: UIEdgeInsets

The amount of space, in pixels, between the border and the contents of the element.

var position: TVElementPosition

A value indicating the position of the element relative to the screen or its containing element.

enum TVElementPosition

Location of an element relative to the screen or its containing element.

### Changing the Text of an Element

var fontSize: CGFloat

The font size applied to any text contained in the element.

var fontWeight: String?

A string indicating how thick or thin the font is.

var maxTextLines: Int

The maximum number of lines of text allowed inside of the element.

var textAlignment: NSTextAlignment

The horizontal alignment of text within an element.

var textHighlightStyle: String?

A string indicating how a label reacts when it is in focus.

var textMinimumScaleFactor: CGFloat

The minimum size text can be if the original text size does not fit in an element.

var textStyle: String?

The style applied to the text in an element.

### Modifying an Image

var imageTreatmentName: String?

A value that determines how an image is displayed.

var ratingStyle: String?

A string indicating the style to be used by a rating element.

### Coloring an Element

var backgroundColor: TVColor?

The background color for an element.

var color: TVColor?

The color for an element.

var highlightColor: TVColor?

The color of the element when it is highlighted.

var tintColor: TVColor?

The tint color applied to an element.

### Element Styles

Transition Style Values

The type of transition to apply to an element.

Rating Style Values

The size of the star image used for a rating element.

Label State Values

How text is displayed when an element is in focus.

Text Style Values

Font size and weight.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Custom Styles

class TVStyleFactory

An object used to register custom style properties.

Deprecated

class TVColor

The color data used by styles.

Deprecated

