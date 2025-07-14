

- BrowserEngineKit
- BEAccessibilityTextMarkerSupport
-  accessibilityContent(for:) 

Instance Method

# accessibilityContent(for:)

Returns the accessibility content for a text range.

iOS 18.2+iPadOS 18.2+macOStvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func accessibilityContent(for range: BEAccessibilityTextMarker.Range) -> String?
```

**Required**

## Parameters 

`range`  

The text marker range.

## Return Value

The string of text within the marker range, or `nil` if there’s no text in the range.

