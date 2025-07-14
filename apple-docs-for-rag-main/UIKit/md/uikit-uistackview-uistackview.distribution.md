

- UIKit
- UIStackView
-  UIStackView.Distribution 

Enumeration

# UIStackView.Distribution

The layout that defines the size and position of the arranged views along the stack view’s axis.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
enum Distribution
```

## Topics

### Constants

case fill

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case fillEqually

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case fillProportionally

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case equalSpacing

A layout where the stack view positions its arranged views so that they fill the available space along the stack view’s axis.

case equalCentering

A layout that attempts to position the arranged views with equal center-to-center spacing along the stack view’s axis, while maintaining the spacing property’s distance between views.

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

enum Alignment

The layout of arranged views perpendicular to the stack view’s axis.

