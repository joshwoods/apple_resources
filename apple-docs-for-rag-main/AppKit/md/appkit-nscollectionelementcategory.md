

- AppKit
-  NSCollectionElementCategory 

Enumeration

# NSCollectionElementCategory

Constants specifying the type of element in the collection view.

Mac Catalyst 13.1+macOS 10.11+

``` source
enum NSCollectionElementCategory
```

## Topics

### Constants

case item

The element is an item. Items represent the main content of your collection view.

case supplementaryView

The element is a supplementary view. Use supplementary views for single views that contain some data but are associated with an entire section. For example, use them to specify header or footer views for a section.

case decorationView

The element is a decoration view. Decoration views represent visual adornments that do not contain any data of their own.

case interItemGap

The element is an inter-item gap. An inter-item gap element is a custom visual indicator that is displayed between items when dropping items into the collection view.

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

### Constants

Inter-Item Gap Support

Constant for supporting inter-item gaps.

