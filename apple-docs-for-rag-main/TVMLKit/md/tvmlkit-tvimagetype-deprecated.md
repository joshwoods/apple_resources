

- TVMLKit
-  TVImageType Deprecated

Enumeration

# TVImageType

The type of image.

tvOS 9.0–18.0Deprecated

``` source
enum TVImageType
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case image

The image is presented in its actual size.

case fullscreen

The image occupies the entire screen.

case decoration

The image is a decoration image, which is used to display an image inside of another image.

case hero

The image is a hero image, which is used to display a product image.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying an Image

var url: URL?

A URL that points to the location of the image.

Deprecated

var imageType: TVImageType

The type of image.

Deprecated

var srcset: [String : URL]?

A dictionary specifying versions of the same image for different resolutions.

Deprecated

