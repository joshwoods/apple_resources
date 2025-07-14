

- UIKit
- UIInputView
-  allowsSelfSizing 

Instance Property

# allowsSelfSizing

A Boolean value that indicates whether the input view is responsible for its own size.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var allowsSelfSizing: Bool { get set }
```

## Discussion

When the value of this property is false (the default), UIKit determines an appropriate size of the input view based on its current layout. When the value of this property is true, UIKit honors the value returned by the systemLayoutSizeFitting(_:) method of the input view.

