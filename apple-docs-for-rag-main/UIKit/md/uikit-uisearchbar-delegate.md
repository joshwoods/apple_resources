

- UIKit
- UISearchBar
-  delegate 

Instance Property

# delegate

The search bar’s delegate object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UISearchBarDelegate)? { get set }
```

## Discussion

The delegate should conform to the UISearchBarDelegate protocol. Set this property to further modify the behavior. The default value is `nil`.

## See Also

### Handling search bar interactions

protocol UISearchBarDelegate

A collection of optional methods that you implement to make a search bar control functional.

