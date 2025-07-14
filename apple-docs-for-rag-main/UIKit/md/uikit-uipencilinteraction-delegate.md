

- UIKit
- UIPencilInteraction
-  delegate 

Instance Property

# delegate

The object that handles the double-tap or squeeze interactions a person makes on Apple Pencil.

iOS 12.1+iPadOS 12.1+Mac Catalyst 13.1+

``` source
@MainActor
weak var delegate: (any UIPencilInteractionDelegate)? { get set }
```

## See Also

### Handling interactions

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

