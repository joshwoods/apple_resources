

- UIKit
- UIPrintInteractionController
-  delegate 

Instance Property

# delegate

The delegate of the print-interaction controller.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIPrintInteractionControllerDelegate)? { get set }
```

## Discussion

The delegate must adopt the UIPrintInteractionControllerDelegate protocol and implement one or more of its methods. It is not retained.

## See Also

### Assigning the delegate

protocol UIPrintInteractionControllerDelegate

An optional set of methods that the delegate of the shared print-interaction controller implements.

