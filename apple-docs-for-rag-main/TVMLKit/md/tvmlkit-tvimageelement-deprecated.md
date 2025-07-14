

- TVMLKit
-  TVImageElement Deprecated

Class

# TVImageElement

A representation of a read-only DOM node containing the attributes that describe an image element.

tvOS 9.0–18.0Deprecated

``` source
class TVImageElement
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Identifying an Image

var url: URL?

A URL that points to the location of the image.

var imageType: TVImageType

The type of image.

enum TVImageType

The type of image.

var srcset: [String : URL]?

A dictionary specifying versions of the same image for different resolutions.

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

class TVTextElement

The textual content for the DOM element.

Deprecated

Creating TVML Elements

Avoid rewriting complex and often used elements by creating a simplified custom element.

