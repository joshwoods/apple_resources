

- UIKit
-  UIToolbarDelegate 

Protocol

# UIToolbarDelegate

The interface that toolbar delegate objects implement to manage the toolbar behavior.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIToolbarDelegate : UIBarPositioningDelegate
```

## Overview

This protocol declares no methods of its own, but conforms to the UIBarPositioningDelegate protocol to support the positioning of a toolbar when it’s moved to a window.

## Relationships

### Inherits From

- NSObjectProtocol
- UIBarPositioningDelegate

## See Also

### Managing toolbar changes

var delegate: (any UIToolbarDelegate)?

The toolbar’s delegate object.

