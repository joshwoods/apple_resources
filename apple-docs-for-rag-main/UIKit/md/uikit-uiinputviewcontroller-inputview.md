

- UIKit
- UIInputViewController
-  inputView 

Instance Property

# inputView

The primary view for the input view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var inputView: UIInputView? { get set }
```

## Discussion

When you use an input view controller subclass as the primary view controller for a custom keyboard, this property’s UIInputView object is initially empty. To display your keyboard’s user interface, add controls and views to the inputView property.

