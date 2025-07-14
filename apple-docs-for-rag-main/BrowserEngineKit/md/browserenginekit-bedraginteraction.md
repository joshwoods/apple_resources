

- BrowserEngineKit
-  BEDragInteraction 

Class

# BEDragInteraction

A `UIDragInteraction` subclass with features specific to browsers to enable asynchronous preparations and behaviours.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
class BEDragInteraction
```

## Overview

An interaction that enables your app to asynchronously provide drag items.

## Overview

`BEDragInteraction` is a subclass of UIDragInteraction that additionally supports asynchronous interaction.

When a person drags a UI element in your browser app, create a `BEDragInteraction` and attach it to the source view. When you create the object, set its delegate to an object that conforms to BEDragInteractionDelegate. Use the delegate to prepare the UIDragSession before the system requests drag items, which it does by calling the delegate’s dragInteraction(_:itemsForBeginning:) method.

## Topics

### Creating a drag interaction

init(delegate: any BEDragInteractionDelegate)

Creates an drag interaction with the specified delegate.

### Handling drag gestures

var delegate: (any BEDragInteractionDelegate)?

The object that manages the drag interaction lifecycle.

protocol BEDragInteractionDelegate

A protocol to which the drag interaction delegates conform.

## Relationships

### Inherits From

- UIDragInteraction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- UIInteraction

## See Also

### Drag interaction

protocol BEDragInteractionDelegate

A protocol to which the drag interaction delegates conform.

