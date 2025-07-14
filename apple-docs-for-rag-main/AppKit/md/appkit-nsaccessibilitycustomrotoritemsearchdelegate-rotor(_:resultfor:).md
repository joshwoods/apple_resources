

- AppKit
- NSAccessibilityCustomRotorItemSearchDelegate
-  rotor(\_:resultFor:) 

Instance Method

# rotor(\_:resultFor:)

Performs a search with the specified search parameters and returns the item result.

macOS 10.13+

``` source
func rotor(
    _ rotor: NSAccessibilityCustomRotor,
    resultFor searchParameters: NSAccessibilityCustomRotor.SearchParameters
) -> NSAccessibilityCustomRotor.ItemResult?
```

**Required**

## See Also

### Finding the Next Item

class SearchParameters

Search parameters for a custom rotor.

