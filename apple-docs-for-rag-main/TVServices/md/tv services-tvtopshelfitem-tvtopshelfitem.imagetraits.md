

- TV Services
- TVTopShelfItem
-  TVTopShelfItem.ImageTraits 

Structure

# TVTopShelfItem.ImageTraits

Constants describing the image format.

tvOS 13.0+

``` source
struct ImageTraits
```

## Topics

### Image Traits

static var screenScale1x: TVTopShelfItem.ImageTraits

An image to display on devices running in a 1x resolution mode.

static var screenScale2x: TVTopShelfItem.ImageTraits

A high-resolution image to display on devices running in a 2x resolution mode.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Providing an Image for the Item

func imageURL(for: TVTopShelfItem.ImageTraits) -> URL?

Returns an image associated with the current item.

func setImageURL(URL?, for: TVTopShelfItem.ImageTraits)

Associates an image with the current item.

