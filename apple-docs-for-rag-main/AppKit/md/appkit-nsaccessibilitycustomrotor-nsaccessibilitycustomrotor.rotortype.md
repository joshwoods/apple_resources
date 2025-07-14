

- AppKit
- NSAccessibilityCustomRotor
-  NSAccessibilityCustomRotor.RotorType 

Enumeration

# NSAccessibilityCustomRotor.RotorType

Constants that indicate the type of content that the rotor represents.

macOS 10.13+

``` source
enum RotorType
```

## Topics

### Constants

case custom

A rotor with a custom label.

case any

Any type of item.

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

case underlinedText

Any underlined text.

case misspelledWord

A misspelled word.

case annotation

An annotation.

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

### Enumeration Cases

case audiograph

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

### Getting the Rotor Type

var type: NSAccessibilityCustomRotor.RotorType

The type of content that the rotor represents.

