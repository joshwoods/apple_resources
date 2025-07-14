

- UIKit
- UIPickerView
-  delegate 

Instance Property

# delegate

The delegate for the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIPickerViewDelegate)? { get set }
```

## Discussion

The delegate must adopt the UIPickerViewDelegate protocol and implement the required methods to return the drawing rectangle for rows in each component. It also provides the content for each component’s row, either as a string or a view, and it typically responds to new selections or deselections.

## See Also

### Customizing the picker behavior

protocol UIPickerViewDelegate

The interface for a picker view’s delegate.

