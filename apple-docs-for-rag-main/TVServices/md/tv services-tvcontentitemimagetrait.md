

- TV Services
-  TVContentItemImageTrait 

Structure

# TVContentItemImageTrait

Traits describing the type of image you want.

tvOS 11.0+

``` source
struct TVContentItemImageTrait
```

## Topics

### Traits

static var screenScale1x: TVContentItemImageTrait

An image meant for a regular display.

static var screenScale2x: TVContentItemImageTrait

An image meant for a Retina display.

static var userInterfaceStyleDark: TVContentItemImageTrait

An image meant for a dark user interface.

static var userInterfaceStyleLight: TVContentItemImageTrait

An image meant for a light user interface.

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

### Accessing Image Resources

var imageURL: URL?

A URL giving the location of the image to be displayed for this content item.

Deprecated

func imageURL(forTraits: TVContentItemImageTrait) -> URL?

Retrieve the URL for the image that best matches the specified traits.

Deprecated

func setImageURL(URL?, forTraits: TVContentItemImageTrait)Deprecated

