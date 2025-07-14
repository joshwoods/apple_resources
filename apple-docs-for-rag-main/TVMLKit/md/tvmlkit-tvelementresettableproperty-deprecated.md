

- TVMLKit
-  TVElementResettableProperty Deprecated

Enumeration

# TVElementResettableProperty

The types of properties that can be reset to their default values.

tvOS 9.0–18.0Deprecated

``` source
enum TVElementResettableProperty
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case updateType

The updateType property is reset to TVElementUpdateType.none.

case autoHighlightIdentifier

The autoHighlightIdentifier property is reset to `nil`.

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

### Resetting a Property’s Value

func resetProperty(TVElementResettableProperty)

Resets the property to its default value.

Deprecated

