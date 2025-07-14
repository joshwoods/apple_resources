

- UIKit
-  UIUserInterfaceLayoutDirection 

Enumeration

# UIUserInterfaceLayoutDirection

Constants that specify the directional flow of the user interface.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum UIUserInterfaceLayoutDirection
```

## Overview

One of these constants is returned by the userInterfaceLayoutDirection property. It indicates the directionality of the language in the user interface of the app.

## Topics

### Constants

case leftToRight

The layout direction is left to right.

case rightToLeft

The layout direction right to left.

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

### Accessing the layout direction

var userInterfaceLayoutDirection: UIUserInterfaceLayoutDirection

The layout direction of the user interface.

