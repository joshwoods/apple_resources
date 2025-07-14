

- Accessibility
- AXCustomContent
-  value 

Instance Property

# value

A localized string that provides a value for the label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var value: String { get }
```

## Discussion

Make the value succinct to work well with assistive technology. For example, either `Portrait` or `Landscape` is an appropriate content value for an `Orientation` label on a photo.

## See Also

### Defining custom content

var label: String

A localized string that identifies the label for this content.

var attributedLabel: NSAttributedString

A localized attributed string that identifies the label for this content.

var attributedValue: NSAttributedString

A localized attributed string that provides a value for the label.

var importance: AXCustomContent.Importance

An object that determines when to output custom accessibility content.

enum Importance

Objects that control the timing of content output.

