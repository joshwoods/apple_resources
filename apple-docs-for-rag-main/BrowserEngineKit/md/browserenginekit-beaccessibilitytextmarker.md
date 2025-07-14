

- BrowserEngineKit
-  BEAccessibilityTextMarker 

Class

# BEAccessibilityTextMarker

An abstract class that represents a location in an element’s accessibility text.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
class BEAccessibilityTextMarker
```

## Overview

Subclass `BEAccessibilityTextMarker` in your app to represent a location in the accessibility text of an element in the document object model (DOM). The system uses your implementation of BEAccessibilityTextMarkerSupport to convert between accessibility text markers and locations in your app’s views, and doesn’t create instances of your subclass or access their data.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

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

func accessibilityTextMarker(forPosition: Int) -> BEAccessibilityTextMarker?

Returns the text marker for the text at a given index in the element’s text.

**Required**

