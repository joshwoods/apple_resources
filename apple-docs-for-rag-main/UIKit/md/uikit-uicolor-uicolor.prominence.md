

- UIKit
- UIColor
-  UIColor.Prominence 

Enumeration

# UIColor.Prominence

A type that indicates the prominence of a color in the interface.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
enum Prominence
```

## Overview

Interface elements, such as text labels, can have a different level of prominence in the UI. For example, a title label appears more prominently than a subtitle or caption. When you specify a label’s color, you can pass one of the UIColor.Prominence constants to withProminence(_:) to communicate how prominently to display that color in the UI.

The following code creates a label with a secondary, vibrant red color:

```
let label = UILabel()
label.preferredVibrancy = .automatic
label.textColor = .systemRed.withProminence(.secondary) 
```

## Topics

### Constants

case primary

A color with a primary prominence, the most prominent in the interface.

case secondary

A color with a secondary prominence.

case tertiary

A color with a tertiary prominence.

case quaternary

A color with a quaternary prominence, the least prominent in the interface.

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

### Working with color prominence

var prominence: UIColor.Prominence

func withProminence(UIColor.Prominence) -> UIColor

Returns the version of the current color that results from applying the specified prominence.

