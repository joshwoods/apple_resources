

- AppKit
- NSCandidateListTouchBarItem
-  client 

Instance Property

# client

The client object for the candidate list item.

macOS 10.12.2+

``` source
@MainActor
weak var client: (any NSView & NSTextInputClient)? { get set }
```

## Discussion

This object must be a subclass of NSView and adopt the NSTextInputClient protocol.

The candidate list item uses this property to show completion candidates as users enter text. You can disable this behavior with the allowsTextInputContextCandidates property.

## See Also

### Providing a client and a delegate

var delegate: (any NSCandidateListTouchBarItemDelegate)?

The delegate of the candidate list item.

protocol NSCandidateListTouchBarItemDelegate

A set of methods that a candidate list item delegate uses to enable selection state and list visibility.

