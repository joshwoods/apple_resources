

- AppKit
- NSCandidateListTouchBarItem
-  delegate 

Instance Property

# delegate

The delegate of the candidate list item.

macOS 10.12.2+

``` source
@MainActor
weak var delegate: (any NSCandidateListTouchBarItemDelegate)? { get set }
```

## See Also

### Providing a client and a delegate

var client: (any NSView &amp; NSTextInputClient)?

The client object for the candidate list item.

protocol NSCandidateListTouchBarItemDelegate

A set of methods that a candidate list item delegate uses to enable selection state and list visibility.

