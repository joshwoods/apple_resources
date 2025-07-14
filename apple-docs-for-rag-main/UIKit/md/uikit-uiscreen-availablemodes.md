

- UIKit
- UIScreen
-  availableModes 

Instance Property

# availableModes

The display modes that can be associated with the screen.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+

``` source
@MainActor
var availableModes: [UIScreenMode] { get }
```

## Mentioned in 

Presenting content on a connected display

## Discussion

The array contains one or more UIScreenMode objects, each of which represents a display mode supported by the screen.

## See Also

### Managing screen modes

var currentMode: UIScreenMode?

The current screen mode associated with the screen.

var preferredMode: UIScreenMode?

The preferred display mode for the screen.

