

- AppKit
-  NSColorChanging 

Protocol

# NSColorChanging

macOS

``` source
protocol NSColorChanging : NSObjectProtocol
```

## Overview

When the user selects a color in an NSColorPanel object, the panel tries to call this method on the first responder. You can override this method in any responder that needs to respond to a color change.

## Topics

### Responding to a Color Change

func changeColor(NSColorPanel?)

Sent to the first responder when the user selects a color in an NSColorPanel object.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextView

## See Also

### Responding to a Color Change

class let colorDidChangeNotification: NSNotification.Name

Posted when the color of the `NSColorPanel` is set, as when NSColorPanel is invoked.

