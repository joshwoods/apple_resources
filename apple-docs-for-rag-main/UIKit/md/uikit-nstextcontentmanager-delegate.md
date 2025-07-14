

- UIKit
- NSTextContentManager
-  delegate 

Instance Property

# delegate

The delegate for the content manager object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
weak var delegate: (any NSTextContentManagerDelegate)? { get set }
```

## See Also

### Customizing and validating text elements

protocol NSTextContentManagerDelegate

The optional methods that delegates of content manager objects implement for customizing or validating text elements.

struct EnumerationOptions

Values that control the order in which the framework enumerates text elements.

