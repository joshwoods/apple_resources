

- UIKit
-  NSTextLineFragment 

Class

# NSTextLineFragment

A class that represents a line fragment as a single textual layout and rendering unit inside a text layout fragment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
class NSTextLineFragment
```

## Topics

### Creating line fragments

init(attributedString: NSAttributedString, range: NSRange)

Creates a new line fragment from the attributed string for the range of characters you specify.

init?(coder: NSCoder)

Creates a new line fragment with from data in an unarchiver.

convenience init(string: String, attributes: [NSAttributedString.Key : Any], range: NSRange)

Creates a new line fragment using the string, attributes, and range you provide.

### Line fragment characteristics

var attributedString: NSAttributedString

The source attributed string.

var characterRange: NSRange

The string range for the source attributed string that corresponds to this line fragment.

var glyphOrigin: CGPoint

Rendering origin for the left-most glyph in the line fragment coordinate system.

var typographicBounds: CGRect

The typographic bounds that specifies the dimensions of the line fragment for laying out line fragments to each other.

### Finding specific text

func characterIndex(for: CGPoint) -> Int

Returns character index for a point inside the line fragment coordinate system.

func fractionOfDistanceThroughGlyph(for: CGPoint) -> CGFloat

Returns character index for a point inside the line fragment coordinate system.

func locationForCharacter(at: Int) -> CGPoint

Returns the location of the character at the specified index.

### Drawing

func draw(at: CGPoint, in: CGContext)

Renders the line fragment contents at the rendering origin.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Layout

Using TextKit 2 to interact with text

Interact with text by managing text selection and inserting custom text elements.

Display text with a custom layout

Lay out text in a custom-shaped container and apply glyph substitutions.

class NSTextLayoutManager

The primary class that you use to manage text layout and presentation for custom text displays.

class NSTextContainer

A region where text layout occurs.

class NSTextLayoutFragment

A class that represents the layout fragment typically corresponding to a rendering surface, such as a layer or view subclass.

class NSTextViewportLayoutController

Manages the layout process inside the viewport interacting with its delegate.

protocol NSTextLayoutOrientationProvider

A set of methods that define the orientation of text for an object.

