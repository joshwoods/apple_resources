

- Shared With You
-  SWHighlightCenterDelegate 

Protocol

# SWHighlightCenterDelegate

The protocol you use to notify the delegate when the list or rank order of surfaced highlights changes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
protocol SWHighlightCenterDelegate : NSObjectProtocol
```

## Topics

### Protocol Attributes

func highlightCenterHighlightsDidChange(SWHighlightCenter)

Notifies the delegate that the list or rank order of surfaced highlights has changed.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the delegate

var delegate: (any SWHighlightCenterDelegate)?

The delegate object for the highlight center.

