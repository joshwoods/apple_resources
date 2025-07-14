

- AppKit
- NSProgressIndicator
-  observedProgress 

Instance Property

# observedProgress

The progress object to use for updating the progress view.

macOS 14.0+

``` source
@MainActor
var observedProgress: Progress? { get set }
```

## Discussion

Set this property when you want the progress view to automatically update its progress value using the information it receives from the Progress object. Setting this property also modifies the isIndeterminate, minValue, maxValue, and doubleValue properties of the indicator. Set the property to `nil` when you want to update the progress manually. The default value of this property is `nil`.

For more information on configuring a progress object, see Progress.

