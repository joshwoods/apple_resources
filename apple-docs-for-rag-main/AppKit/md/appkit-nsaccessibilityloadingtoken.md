

- AppKit
-  NSAccessibilityLoadingToken 

Type Alias

# NSAccessibilityLoadingToken

A token type for loading accessibility elements.

macOS

``` source
typealias NSAccessibilityLoadingToken = any NSSecureCoding & NSObjectProtocol
```

## See Also

### Supporting Accessibility

func accessibilityElement(withToken: NSAccessibilityLoadingToken) -> (any NSAccessibilityElementProtocol)?

Loads the target accessibility element with the specified load token.

**Required**

func accessibilityRangeInTargetElement(withToken: NSAccessibilityLoadingToken) -> NSRange

Returns the range that specifies the area of interest in text-based accessibility elements with the specified load token.

