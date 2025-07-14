

- TVMLKit
-  TVTextElement Deprecated

Class

# TVTextElement

The textual content for the DOM element.

tvOS 9.0–18.0Deprecated

``` source
class TVTextElement
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Creating Attributed Strings

func makeAttributedString(font: UIFont) -> NSAttributedString

Provides an attributed string for a given font.

func makeAttributedString(font: UIFont, foregroundColor: UIColor?, textAlignment: NSTextAlignment) -> NSAttributedString

Convenience method for configuring an attributed string given the specified attributes.

### Inspecting Text Elements

var attributedString: NSAttributedString?

The text for an element.

var textStyle: TVTextElementStyle

The style applied to the text of the element.

enum TVTextElementStyle

The style applied to the text inside of an element.

## Relationships

### Inherits From

- TVViewElement

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Custom Elements

class TVElementFactory

An object used to register new elements to extend the Apple TV Markup Language (TVML).

Deprecated

class TVImageElement

A representation of a read-only DOM node containing the attributes that describe an image element.

Deprecated

Creating TVML Elements

Avoid rewriting complex and often used elements by creating a simplified custom element.

