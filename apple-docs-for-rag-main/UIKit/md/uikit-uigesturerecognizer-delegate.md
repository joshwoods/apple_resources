

- UIKit
- UIGestureRecognizer
-  delegate 

Instance Property

# delegate

The delegate of the gesture recognizer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIGestureRecognizerDelegate)? { get set }
```

## Discussion

The gesture recognizer maintains a weak reference to its delegate. The delegate must adopt the UIGestureRecognizerDelegate protocol and implement one or more of its methods.

## See Also

### Managing gesture-related interactions

protocol UIGestureRecognizerDelegate

A set of methods implemented by the delegate of a gesture recognizer to fine-tune an app’s gesture-recognition behavior.

