

- AppKit
- NSAccessibilityElementLoading
-  accessibilityElement(withToken:) 

Instance Method

# accessibilityElement(withToken:)

Loads the target accessibility element with the specified load token.

macOS 10.13+

``` source
func accessibilityElement(withToken token: NSAccessibilityLoadingToken) -> (any NSAccessibilityElementProtocol)?
```

**Required**

## See Also

### Supporting Accessibility

func accessibilityRangeInTargetElement(withToken: NSAccessibilityLoadingToken) -> NSRange

Returns the range that specifies the area of interest in text-based accessibility elements with the specified load token.

typealias NSAccessibilityLoadingToken

A token type for loading accessibility elements.

