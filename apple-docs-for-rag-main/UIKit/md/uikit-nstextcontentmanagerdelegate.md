

- UIKit
-  NSTextContentManagerDelegate 

Protocol

# NSTextContentManagerDelegate

The optional methods that delegates of content manager objects implement for customizing or validating text elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
protocol NSTextContentManagerDelegate : NSObjectProtocol
```

## Topics

### Finding a text element at a specific location

func textContentManager(NSTextContentManager, textElementAt: any NSTextLocation) -> NSTextElement?

The method the framework calls to return the text element at a specific location.

### Validating a text element

func textContentManager(NSTextContentManager, shouldEnumerate: NSTextElement, options: NSTextContentManager.EnumerationOptions) -> Bool

Returns a Boolean value that indicates whether the framework should skip this text element in the enumeration.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSTextContentStorageDelegate

## See Also

### Customizing and validating text elements

var delegate: (any NSTextContentManagerDelegate)?

The delegate for the content manager object.

struct EnumerationOptions

Values that control the order in which the framework enumerates text elements.

