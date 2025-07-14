

- Accessibility
- AXCustomContent
-  AXCustomContent.Importance 

Enumeration

# AXCustomContent.Importance

Objects that control the timing of content output.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum Importance
```

## Topics

### Creating a content importance enumeration

init?(rawValue: UInt)

### Setting content importance

case `default`

Output the content to the user on demand.

case high

Output the content to the user immediately.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Defining custom content

var label: String

A localized string that identifies the label for this content.

var attributedLabel: NSAttributedString

A localized attributed string that identifies the label for this content.

var value: String

A localized string that provides a value for the label.

var attributedValue: NSAttributedString

A localized attributed string that provides a value for the label.

var importance: AXCustomContent.Importance

An object that determines when to output custom accessibility content.

