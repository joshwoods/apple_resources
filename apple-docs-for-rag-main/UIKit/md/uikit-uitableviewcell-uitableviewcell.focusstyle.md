

- UIKit
- UITableViewCell
-  UITableViewCell.FocusStyle 

Enumeration

# UITableViewCell.FocusStyle

The style of focused cells.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
enum FocusStyle
```

## Overview

You use these constants to set the value of the focusStyle property.

## Topics

### Constants

case `default`

The cell alters its appearance in a standard, system-defined way when it becomes focused.

case custom

The cell doesn’t alter its appearance automatically when it becomes focused.

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

### Managing focus

var focusStyle: UITableViewCell.FocusStyle

The appearance of the cell when focused.

