

- BrowserEngineKit
- BEAccessibilityTextMarkerSupport
-  accessibilityTextMarkerRange(for:) 

Instance Method

# accessibilityTextMarkerRange(for:)

Returns the text marker range for the text in a given range.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func accessibilityTextMarkerRange(for range: NSRange) -> BEAccessibilityTextMarker.Range?
```

**Required**

## Parameters 

`range`  

A range of text in the element’s string.

## Return Value

The text marker range for the text in `range`, or `nil` if the method can’t calculate the range.

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

func accessibilityRange(for: BEAccessibilityTextMarker.Range) -> NSRange

Returns the range for the text in a given accessibility marker range.

**Required**

class Range

A class that represents a range in an element’s accessibility text.

