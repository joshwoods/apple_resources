

- Accessibility
- AXCustomContent
-  importance 

Instance Property

# importance

An object that determines when to output custom accessibility content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var importance: AXCustomContent.Importance { get set }
```

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

enum Importance

Objects that control the timing of content output.

