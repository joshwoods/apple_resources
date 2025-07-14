

- AppKit
- NSAccessibilityCustomRotor
-  itemLoadingDelegate 

Instance Property

# itemLoadingDelegate

The delegate for loading item results that don’t have a backing UI element at loading time.

macOS 10.13+

``` source
weak var itemLoadingDelegate: (any NSAccessibilityElementLoading)? { get set }
```

## See Also

### Loading the Item

protocol NSAccessibilityElementLoading

A role-based protocol that declares the minimum interface necessary for an accessibility element to support loading.

