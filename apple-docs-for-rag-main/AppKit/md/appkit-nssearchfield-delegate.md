

- AppKit
- NSSearchField
-  delegate 

Instance Property

# delegate

The delegate for the search field, or `nil` if the search field doesn’t have a delegate.

macOS 10.11+

``` source
@MainActor
weak var delegate: (any NSSearchFieldDelegate)? { get set }
```

## See Also

### Managing Search

protocol NSSearchFieldDelegate

A protocol that a search field delegate can use to determine when a search started or ended.

