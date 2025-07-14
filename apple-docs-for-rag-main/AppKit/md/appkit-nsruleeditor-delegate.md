

- AppKit
- NSRuleEditor
-  delegate 

Instance Property

# delegate

The rule editor’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSRuleEditorDelegate)? { get set }
```

## See Also

### Configuring the Delegate

protocol NSRuleEditorDelegate

The `NSRuleEditorDelegate` protocol defines the optional methods implemented by delegates of NSRuleEditor objects.

