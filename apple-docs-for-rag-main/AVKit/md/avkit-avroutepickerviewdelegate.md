

- AVKit
-  AVRoutePickerViewDelegate 

Protocol

# AVRoutePickerViewDelegate

A protocol that defines the methods to adopt to respond to route picker view presentation events.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+

``` source
protocol AVRoutePickerViewDelegate : NSObjectProtocol
```

## Topics

### Presenting Routes

func routePickerViewWillBeginPresentingRoutes(AVRoutePickerView)

Tells the delegate that the route picker view is about to begin presenting routes to the user.

func routePickerViewDidEndPresentingRoutes(AVRoutePickerView)

Tells the delegate when the route picker view finishes presenting routes to the user.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring the delegate

var delegate: (any AVRoutePickerViewDelegate)?

The delegate object for the route picker.

