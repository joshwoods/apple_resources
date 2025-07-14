

- TVMLKit
-  TVViewElementStyleType Deprecated

Enumeration

# TVViewElementStyleType

Describes the different style types for an element.

tvOS 9.0–18.0Deprecated

``` source
enum TVViewElementStyleType
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case integer

An NSNumber value.

case double

An NSNumber value.

case point

A CGPoint value.

case string

A NSString value.

case color

A TVColor value.

case URL

A NSURL value.

case edgeInsets

An UIEdgeInsets value.

### Enumeration Cases

case transform

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

### Creating New Style Properties

class func registerStyleName(String, type: TVViewElementStyleType, inherited: Bool)

Creates a new style property of the indicated type.

Deprecated

