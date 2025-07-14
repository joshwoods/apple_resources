

- AppKit
-  NSTextContentStorageDelegate 

Protocol

# NSTextContentStorageDelegate

The optional methods that delegates of content storage objects implement to handle content processing.

macOS 12.0+

``` source
protocol NSTextContentStorageDelegate : NSTextContentManagerDelegate
```

## Topics

### Working with paragraphs

func textContentStorage(NSTextContentStorage, textParagraphWith: NSRange) -> NSTextParagraph?

Returns a custom paragraph for a range that you provide from the object’s attributed string.

## Relationships

### Inherits From

- NSObjectProtocol
- NSTextContentManagerDelegate

## See Also

### Accessing paragraphs

var delegate: (any NSTextContentStorageDelegate)?

The delegate for the content storage object.

