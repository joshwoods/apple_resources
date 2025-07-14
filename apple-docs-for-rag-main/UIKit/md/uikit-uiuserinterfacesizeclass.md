

- UIKit
-  UIUserInterfaceSizeClass 

Enumeration

# UIUserInterfaceSizeClass

Constants that indicate the size class of a view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum UIUserInterfaceSizeClass
```

## Topics

### Constants

case unspecified

Indicates the size class hasn’t been specified.

case compact

Indicates a compact size class.

case regular

Indicates a regular size class.

### Initializers

init(UserInterfaceSizeClass?)

Creates a size class from the specified SwiftUI size class.

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving size class traits

var horizontalSizeClass: UIUserInterfaceSizeClass

The horizontal size class of the trait collection.

var verticalSizeClass: UIUserInterfaceSizeClass

The vertical size class of the trait collection.

