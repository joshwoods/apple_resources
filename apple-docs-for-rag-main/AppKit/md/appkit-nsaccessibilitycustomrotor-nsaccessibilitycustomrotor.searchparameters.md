

- AppKit
- NSAccessibilityCustomRotor
-  NSAccessibilityCustomRotor.SearchParameters 

Class

# NSAccessibilityCustomRotor.SearchParameters

Search parameters for a custom rotor.

macOS 10.13+

``` source
class SearchParameters
```

## Overview

Use these parameters to determine the next matching NSAccessibilityCustomRotor.ItemResult.

## Topics

### Managing the Current Item

var currentItem: NSAccessibilityCustomRotor.ItemResult?

The current item that determines where the search starts.

class ItemResult

A target accessibility element that a custom rotor references.

### Specifying the Filter String

var filterString: String

A string of text to filter the results against.

### Specifying Search Direction

var searchDirection: NSAccessibilityCustomRotor.SearchDirection

The direction to search for an item result.

enum SearchDirection

Constants that describe the direction to search for an item result.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Finding the Next Item

func rotor(NSAccessibilityCustomRotor, resultFor: NSAccessibilityCustomRotor.SearchParameters) -> NSAccessibilityCustomRotor.ItemResult?

Performs a search with the specified search parameters and returns the item result.

**Required**

