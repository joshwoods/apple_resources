

- Notification Center
- NCWidgetSearchViewController
-  delegate Deprecated

Instance Property

# delegate

The search view controller’s delegate or `nil` if the receiver doesn’t have a delegate.

macOS 10.10–11.0Deprecated

``` source
@IBOutlet @MainActor
weak var delegate: (any NCWidgetSearchViewDelegate)? { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

A search view controller’s delegate performs a search on the input term and updates the controller’s searchResults property with the results.

## See Also

### Enabling Search

protocol NCWidgetSearchViewDelegate

The interface for enabling user searches in the search view controller of a macOS Today widget.

Deprecated

