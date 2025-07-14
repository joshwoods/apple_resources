

- BrowserEngineKit
- BEAccessibilityTextMarkerSupport
-  accessibilityTextMarkerRangeForCurrentSelection() 

Instance Method

# accessibilityTextMarkerRangeForCurrentSelection()

The text marker range of the current selection.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func accessibilityTextMarkerRangeForCurrentSelection() -> BEAccessibilityTextMarker.Range?
```

**Required**

## Overview

If there’s no text selected in the element, return `nil`.

## See Also

### Text ranges

func accessibilityBounds(for: BEAccessibilityTextMarker.Range) -> CGRect

Calculates the bounding rectangle for a text range.

**Required**

func accessibilityTextMarkerRange() -> BEAccessibilityTextMarker.Range

The text marker range of the current element.

**Required**

func accessibilityTextMarkerRange(for: NSRange) -> BEAccessibilityTextMarker.Range?

Returns the text marker range for the text in a given range.

**Required**

func accessibilityRange(for: BEAccessibilityTextMarker.Range) -> NSRange

Returns the range for the text in a given accessibility marker range.

**Required**

class Range

A class that represents a range in an element’s accessibility text.

