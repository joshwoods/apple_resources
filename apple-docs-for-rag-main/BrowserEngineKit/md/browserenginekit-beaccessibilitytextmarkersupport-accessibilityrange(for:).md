

- BrowserEngineKit
- BEAccessibilityTextMarkerSupport
-  accessibilityRange(for:) 

Instance Method

# accessibilityRange(for:)

Returns the range for the text in a given accessibility marker range.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func accessibilityRange(for range: BEAccessibilityTextMarker.Range) -> NSRange
```

**Required**

## Parameters 

`range`  

A text marker range for text in the element’s string.

## Return Value

The range in the string for the text in `range`, or `(NSNotFound,0)` if the method can’t calculate the range.

## See Also

### Text ranges

func accessibilityBounds(for: BEAccessibilityTextMarker.Range) -> CGRect

Calculates the bounding rectangle for a text range.

**Required**

func accessibilityTextMarkerRange() -> BEAccessibilityTextMarker.Range

The text marker range of the current element.

**Required**

func accessibilityTextMarkerRangeForCurrentSelection() -> BEAccessibilityTextMarker.Range?

The text marker range of the current selection.

**Required**

func accessibilityTextMarkerRange(for: NSRange) -> BEAccessibilityTextMarker.Range?

Returns the text marker range for the text in a given range.

**Required**

class Range

A class that represents a range in an element’s accessibility text.

