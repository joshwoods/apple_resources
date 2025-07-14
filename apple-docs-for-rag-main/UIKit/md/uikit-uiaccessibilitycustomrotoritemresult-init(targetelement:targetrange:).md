

- UIKit
- UIAccessibilityCustomRotorItemResult
-  init(targetElement:targetRange:) 

Initializer

# init(targetElement:targetRange:)

Creates a rotor item result from the specified target element and text range.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init(
    targetElement: any NSObjectProtocol,
    targetRange: UITextRange?
)
```

## Parameters 

`targetElement`  

The target element of the rotor.

`targetRange`  

The text range for an element that contains text, such as a text view.

## Return Value

An initialized rotor item result.

