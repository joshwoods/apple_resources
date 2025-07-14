

- AVKit
- AVRoutePickerView
-  delegate 

Instance Property

# delegate

The delegate object for the route picker.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+

``` source
@MainActor
weak var delegate: (any AVRoutePickerViewDelegate)? { get set }
```

## See Also

### Configuring the delegate

protocol AVRoutePickerViewDelegate

A protocol that defines the methods to adopt to respond to route picker view presentation events.

