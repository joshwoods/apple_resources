

- BrowserEngineKit
- BEAccessibilityTextMarkerSupport
-  accessibilityBounds(for:) 

Instance Method

# accessibilityBounds(for:)

Calculates the bounding rectangle for a text range.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func accessibilityBounds(for range: BEAccessibilityTextMarker.Range) -> CGRect
```

**Required**

## Parameters 

`range`  

The text marker range.

## Return Value

The bounds in accessiblity space of the text range, or CGRectZero if the method can’t calculate the bounds.

## See Also

### Text ranges

func accessibilityTextMarkerRange() -> BEAccessibilityTextMarker.Range

The text marker range of the current element.

**Required**

func accessibilityTextMarkerRangeForCurrentSelection() -> BEAccessibilityTextMarker.Range?

The text marker range of the current selection.

**Required**

func accessibilityTextMarkerRange(for: NSRange) -> BEAccessibilityTextMarker.Range?

Returns the text marker range for the text in a given range.

**Required**

func accessibilityRange(for: BEAccessibilityTextMarker.Range) -> NSRange

Returns the range for the text in a given accessibility marker range.

**Required**

class Range

A class that represents a range in an element’s accessibility text.

