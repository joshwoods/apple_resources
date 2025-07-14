

- UIKit
-  UIPointerInteraction 

Class

# UIPointerInteraction

An interaction that enables support for effects on a view or customizes the pointer’s appearance within a region of an app.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class UIPointerInteraction
```

## Overview

If you use a UIButton as an interface object, use the button’s isPointerInteractionEnabled and pointerStyleProvider to customize the proposed effect before constructing your own custom pointer effect using a UIPointerInteraction.

Note

In iPadOS, the visual interactions when using mouse or trackpad input versus Apple Pencil input are slightly different: For example, pointer styles such as the system pointer aren’t visible while using Apple Pencil. However, both input devices support effect-based pointers, but have a slightly different visual appearance depending on which device is in use.

## Topics

### Create pointer interactions

init(delegate: (any UIPointerInteractionDelegate)?)

Initializes a pointer interaction object with a specified delegate object.

### Manage pointer interactions

var delegate: (any UIPointerInteractionDelegate)?

An object that responds to pointer movements.

protocol UIPointerInteractionDelegate

An interface for handling pointer movements within the interaction’s view.

### Activate pointer interactions

var isEnabled: Bool

A Boolean value that indicates whether the pointer interaction is an enabled state.

### Trigger a pointer update

func invalidate()

Causes the interaction to update the pointer in response to an event.

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
- UIInteraction

## See Also

### Essentials

protocol UIPointerInteractionDelegate

An interface for handling pointer movements within the interaction’s view.

Integrating pointer interactions into your iPad app

Support touch interactions in your iPad app by adding pointer interactions to your views.

Enhancing your iPad app with pointer interactions

Provide a great user experience with pointing devices, by incorporating pointer content effects and shape customizations.

