

- Accessibility
-  AXCustomContent 

Class

# AXCustomContent

Objects that define custom content and the timing of its output.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class AXCustomContent
```

## Overview

An `AXCustomContent` object contains the accessibility strings for the labels you apply to your accessibility content. Combine them with the AXCustomContentProvider protocol to allow your users to experience the content in a more appropriate manner for each assistive technology.

## Topics

### Creating custom content

convenience init(attributedLabel: NSAttributedString, attributedValue: NSAttributedString)

Creates new custom content with an attributed string and attributed value.

convenience init(label: String, value: String)

Creates new custom content with a label and value.

init?(coder: NSCoder)

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

enum Importance

Objects that control the timing of content output.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Custom accessibility content

protocol AXCustomContentProvider

The interface for customizing the accessibility content.

typealias AXCustomContentReturnBlock

