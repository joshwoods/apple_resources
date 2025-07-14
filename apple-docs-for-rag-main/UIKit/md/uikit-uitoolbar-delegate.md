

- UIKit
- UIToolbar
-  delegate 

Instance Property

# delegate

The toolbar’s delegate object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIToolbarDelegate)? { get set }
```

## Discussion

The delegate should conform to the `UIToolbarDelegate` protocol. You may not set the delegate when the toolbar is managed by a navigation controller. The default value is `nil`.

## See Also

### Managing toolbar changes

protocol UIToolbarDelegate

The interface that toolbar delegate objects implement to manage the toolbar behavior.

