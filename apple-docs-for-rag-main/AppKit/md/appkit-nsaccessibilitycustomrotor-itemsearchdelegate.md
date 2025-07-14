

- AppKit
- NSAccessibilityCustomRotor
-  itemSearchDelegate 

Instance Property

# itemSearchDelegate

The delegate for finding the next item result.

macOS 10.13+

``` source
weak var itemSearchDelegate: (any NSAccessibilityCustomRotorItemSearchDelegate)? { get set }
```

## See Also

### Navigating to the Next Item

protocol NSAccessibilityCustomRotorItemSearchDelegate

A delegate for a custom rotor that finds the next item result after performing a search with the specified search parameters.

