

- AppKit
- NSAccessibilityElementLoading
-  accessibilityRangeInTargetElement(withToken:) 

Instance Method

# accessibilityRangeInTargetElement(withToken:)

Returns the range that specifies the area of interest in text-based accessibility elements with the specified load token.

macOS 10.13+

``` source
optional func accessibilityRangeInTargetElement(withToken token: NSAccessibilityLoadingToken) -> NSRange
```

## See Also

### Supporting Accessibility

func accessibilityElement(withToken: NSAccessibilityLoadingToken) -> (any NSAccessibilityElementProtocol)?

Loads the target accessibility element with the specified load token.

**Required**

typealias NSAccessibilityLoadingToken

A token type for loading accessibility elements.

