

- UIKit
- UIAccessibilityIdentification
-  accessibilityIdentifier 

Instance Property

# accessibilityIdentifier

A string that identifies the element.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityIdentifier: String? { get set }
```

**Required**

## Discussion

An identifier can be used to uniquely identify an element in the scripts you write using the UI Automation interfaces. Using an identifier allows you to avoid inappropriately setting or accessing an element’s accessibility label.

