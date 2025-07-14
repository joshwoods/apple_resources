

- AppKit
- NSTabView
-  delegate 

Instance Property

# delegate

The tab view’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSTabViewDelegate)? { get set }
```

## Discussion

The value of this property must conform to the NSTabViewDelegate protocol.

## See Also

### Handling the Selection of Tabs

protocol NSTabViewDelegate

The `NSTabViewDelegate` protocol defines the optional methods implemented by delegates of `NSTabView` objects.

