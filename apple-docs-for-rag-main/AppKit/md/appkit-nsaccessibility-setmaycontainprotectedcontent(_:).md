

- AppKit
- NSAccessibility
-  setMayContainProtectedContent(\_:) 

Type Method

# setMayContainProtectedContent(\_:)

Sets whether the app may have protected content.

macOS

``` source
static func setMayContainProtectedContent(_ flag: Bool) -> Bool
```

## Discussion

Uses the value of `flag` to specify whether the app may have protected content. Protected content is identified by a value of true for `NSAccessibilityContainsProtectedContentAttribute`, but if `NSAccessibilitySetMayContainProtectedContent` returns false, the value of `NSAccessibilityContainsProtectedContentAttribute` is ignored. This function returns true on success.

