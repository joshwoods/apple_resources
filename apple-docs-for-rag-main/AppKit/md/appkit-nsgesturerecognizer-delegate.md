

- AppKit
- NSGestureRecognizer
-  delegate 

Instance Property

# delegate

The delegate of the gesture recognizer.

macOS 10.10+

``` source
@MainActor
weak var delegate: (any NSGestureRecognizerDelegate)? { get set }
```

## Discussion

Use the delegate for fine-grained control over the recognition of a gesture. For example, you can use the delegate to determine whether gesture recognition should begin or whether it should start only after other gesture recognizers fail.

The delegate must implement the NSGestureRecognizerDelegate protocol.

