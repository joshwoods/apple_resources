

- TV Services
-  TVTopShelfContentStyle Deprecated

Enumeration

# TVTopShelfContentStyle

An enumerated type used to specify the style in which you want your content to be displayed.

tvOS 9.0–13.0Deprecated

``` source
enum TVTopShelfContentStyle
```

Deprecated

TVTopShelfProvider has been replaced by TVTopShelfContent

## Topics

### Constants

case inset

When the using the inset style, your extension should return a flat array of TV content items. The images of the content items will take up most of the area of the Top Shelf, which will slowly rotate through the items.

case sectioned

When using the sectioned style, your extension should return an array that contains content items that represent sections. Each section object should have an array of content items that represent the available media in that section.

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

### Implementing TV Services Extension Properties

var topShelfItems: [TVContentItem]

Returns an array of content items to be displayed.

**Required**

Deprecated

var topShelfStyle: TVTopShelfContentStyle

The user interface style that should be used to display the content items.

**Required**

Deprecated

