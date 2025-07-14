

- AppKit
- NSTextContentManager
-  NSTextContentManager.EnumerationOptions 

Structure

# NSTextContentManager.EnumerationOptions

Values that control the order in which the framework enumerates text elements.

macOS 12.0+

``` source
struct EnumerationOptions
```

## Topics

### Creating text element provider enumeration options

init(rawValue: UInt)

Creates a new text element provider with the provided raw value.

### Accessing the enumeration setting

static var reverse: NSTextContentManager.EnumerationOptions

Returns whether enumerations start from the end of the text element.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Customizing and validating text elements

var delegate: (any NSTextContentManagerDelegate)?

The delegate for the content manager object.

protocol NSTextContentManagerDelegate

The optional methods that delegates of content manager objects implement for customizing or validating text elements.

