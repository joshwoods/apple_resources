

- UIKit
- UIAccessibilityCustomRotor
-  UIAccessibilityCustomRotor.SystemRotorType 

Enumeration

# UIAccessibilityCustomRotor.SystemRotorType

Constants that indicate the type of content that the rotor represents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum SystemRotorType
```

## Topics

### Constants

case none

No specific type.

case link

A link.

case visitedLink

A visited link.

case heading

Any heading-level text.

case headingLevel1

A first-level heading.

case headingLevel2

A second-level heading.

case headingLevel3

A third-level heading.

case headingLevel4

A fourth-level heading.

case headingLevel5

A fifth-level heading.

case headingLevel6

A sixth-level heading.

case boldText

Any bold text.

case italicText

Any italicized text.

case underlineText

Any underlined text.

case misspelledWord

A misspelled word.

case image

An image.

case textField

A text field.

case table

A table of information.

case list

A list of items.

case landmark

A landmark.

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

### Getting the rotor type

var systemRotorType: UIAccessibilityCustomRotor.SystemRotorType

The type of content that the rotor searches.

