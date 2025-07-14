

- AppKit
- NSTextContentStorage
-  delegate 

Instance Property

# delegate

The delegate for the content storage object.

macOS 12.0+

``` source
weak var delegate: (any NSTextContentStorageDelegate)? { get set }
```

## See Also

### Accessing paragraphs

protocol NSTextContentStorageDelegate

The optional methods that delegates of content storage objects implement to handle content processing.

