

- BrowserEngineKit
- BEDragInteraction
-  delegate 

Instance Property

# delegate

The object that manages the drag interaction lifecycle.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
weak var delegate: (any BEDragInteractionDelegate)? { get }
```

## Discussion

The drag interaction’s delegate object.

## Overview

The delegate conforms to BEDragInteractionDelegate.

## See Also

### Handling drag gestures

protocol BEDragInteractionDelegate

A protocol to which the drag interaction delegates conform.

