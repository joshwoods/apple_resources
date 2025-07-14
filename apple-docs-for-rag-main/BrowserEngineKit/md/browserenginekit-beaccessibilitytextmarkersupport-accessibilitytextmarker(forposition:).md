

- BrowserEngineKit
- BEAccessibilityTextMarkerSupport
-  accessibilityTextMarker(forPosition:) 

Instance Method

# accessibilityTextMarker(forPosition:)

Returns the text marker for the text at a given index in the element’s text.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func accessibilityTextMarker(forPosition position: Int) -> BEAccessibilityTextMarker?
```

**Required**

## Parameters 

`position`  

An index into the element’s text.

## Return Value

The text marker for the text at `position`, or `nil` if there isn’t text at that position.

## See Also

### Text positions

func accessibilityNextTextMarker(BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that follows the given text marker.

**Required**

func accessibilityPreviousTextMarker(BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that precedes the given text marker.

**Required**

func accessibilityLineStartMarker(for: BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that represents the start of the line that contains the given text marker.

**Required**

func accessibilityLineEndMarker(for: BEAccessibilityTextMarker) -> BEAccessibilityTextMarker?

Returns the text marker that represents the end of the line that contains the given text marker.

**Required**

func accessibilityMarker(for: CGPoint) -> BEAccessibilityTextMarker?

Returns the text marker at a point in the view’s coordinate system.

**Required**

class BEAccessibilityTextMarker

An abstract class that represents a location in an element’s accessibility text.

