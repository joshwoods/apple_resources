

- UIKit
- UIAccessibilityElement
-  isAccessibilityElement 

Instance Property

# isAccessibilityElement

A Boolean value indicating whether the item is an accessibility element an assistive application can access.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isAccessibilityElement: Bool { get set }
```

## Discussion

The default value for this property is false. If the receiver is a UIKit control, the default value is true.

