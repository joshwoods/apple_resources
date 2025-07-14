

- AppKit
-  NSAccessibilityCustomRotorItemSearchDelegate 

Protocol

# NSAccessibilityCustomRotorItemSearchDelegate

A delegate for a custom rotor that finds the next item result after performing a search with the specified search parameters.

macOS 10.13+

``` source
protocol NSAccessibilityCustomRotorItemSearchDelegate : NSObjectProtocol
```

## Topics

### Finding the Next Item

func rotor(NSAccessibilityCustomRotor, resultFor: NSAccessibilityCustomRotor.SearchParameters) -> NSAccessibilityCustomRotor.ItemResult?

Performs a search with the specified search parameters and returns the item result.

**Required**

class SearchParameters

Search parameters for a custom rotor.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Navigating to the Next Item

var itemSearchDelegate: (any NSAccessibilityCustomRotorItemSearchDelegate)?

The delegate for finding the next item result.

