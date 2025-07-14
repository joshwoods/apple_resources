

- UIKit
-  UIPreviewInteraction 

Class

# UIPreviewInteraction

A class that registers a view to provide a custom user experience in response to 3D Touch interactions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPreviewInteraction
```

## Overview

A 3D Touch interaction results in a *preview interaction* that comprises two phases, the first also called *preview*, followed by *commit*. The interaction progresses through these phases as a person applies more force with a touch. The following image shows the relationship between the force of a person’s touch and the phases of the preview interaction.

When using view controller previewing, *peek* represents the preview phase, and *pop* the commit phase.

Note

If you want to provide the system default view controller previewing behavior (*peek* and *pop*), use the registerForPreviewing(with:sourceView:) and unregisterForPreviewing(withContext:) methods on UIViewController instead of UIPreviewInteraction. See `Working With 3D Touch Previews and Preview Quick Actions` for further details.

A preview interaction is responsible for managing 3D Touch interactions for a specified view. It uses a delegate object to communicate the progress and status of the interaction to your code.

To use a preview interaction in your app:

1.  Create a UIPreviewInteraction object, passing the view into the default initializer.

2.  Create a delegate object that conforms to the UIPreviewInteractionDelegate protocol, and implement the appropriate methods.

3.  Assign the delegate object to the delegate property on the preview interaction object.

For more information about the state transitions through which a preview interaction progresses, see UIPreviewInteractionDelegate.

## Topics

### Creating a preview interaction

init(view: UIView)

Returns a newly initialized preview interaction for the specified view.

### Preparing preview interactions

var delegate: (any UIPreviewInteractionDelegate)?

An object that acts as the delegate of the preview interaction.

protocol UIPreviewInteractionDelegate

A set of methods for communicating the progress of a preview interaction.

### Handling preview interactions

var view: UIView?

The view from which the preview interaction receives touch events.

func cancel()

Cancels the current preview interaction.

func location(in: (any UICoordinateSpace)?) -> CGPoint

Returns the location of the touch that started the interaction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### 3D Touch interactions

protocol UIPreviewInteractionDelegate

A set of methods for communicating the progress of a preview interaction.

protocol UIPreviewActionItem

A set of methods that defines the styles you can apply to peek quick actions and peek quick action groups, and defines a read-only accessor for the user-visible title of a peek quick action.

