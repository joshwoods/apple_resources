

- TV Services
- TVTopShelfSectionedItem
-  TVTopShelfSectionedItem.ImageShape 

Enumeration

# TVTopShelfSectionedItem.ImageShape

Constants indicating the aspect ratio of an image.

tvOS 13.0+

``` source
enum ImageShape
```

## Topics

### Image Shapes

case square

An image with a 1:1 aspect ratio.

case poster

A poster-shaped image with a 2:3 aspect ratio.

case hdtv

An image with a 16:9 aspect ratio.

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

### Getting the Image Size Information

class func imageSize(for: TVTopShelfSectionedItem.ImageShape) -> CGSize

Returns the dimensions to use for images of the specified shape.

