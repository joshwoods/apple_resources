

- UIKit
-  UIPencilInteraction 

Class

# UIPencilInteraction

An interaction that tells your app when a person double-taps or squeezes Apple Pencil.

iOS 12.1+iPadOS 12.1+Mac Catalyst 13.1+

``` source
@MainActor
class UIPencilInteraction
```

## Overview

People can interact with certain models of Apple Pencil with a double tap or squeeze. To detect the double tap or squeeze in your app, create a UIPencilInteraction object with a corresponding delegate object. Then, add the interaction to your app’s view. When a person double-taps or squeezes Apple Pencil, the interaction calls the delegate’s corresponding pencilInteraction(_:didReceiveTap:) or pencilInteraction(_:didReceiveSqueeze:) method.

For more information, read Handling double taps from Apple Pencil and Handling squeezes from Apple Pencil.

## Topics

### Creating interactions

init(delegate: any UIPencilInteractionDelegate)

Creates an interaction with the specified delegate.

### Handling interactions

var delegate: (any UIPencilInteractionDelegate)?

The object that handles the double-tap or squeeze interactions a person makes on Apple Pencil.

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

### Enabling interactions

var isEnabled: Bool

A Boolean value that specifies whether the system reports double taps or squeezes on Apple Pencil to your app.

### Determining preferences for actions

class var preferredTapAction: UIPencilPreferredAction

A person’s preferred double-tap action for Apple Pencil, as specified in the Settings app.

class var preferredSqueezeAction: UIPencilPreferredAction

A person’s preferred squeeze action for Apple Pencil, as specified in the Settings app.

enum UIPencilPreferredAction

The actions Apple Pencil can perform after a person performs a double tap or squeeze.

### Determining input type

class var prefersPencilOnlyDrawing: Bool

A person’s preference for drawing with Apple Pencil only, as specified in the Settings app or the system tool picker.

### Determining hover preview preferences

class var prefersHoverToolPreview: Bool

A person’s preference for whether holding a supported model of Apple Pencil close to the screen shows a preview of the current drawing tool, as specified in the Settings app.

### Supporting types

class Tap

An interaction that represents a double tap on Apple Pencil.

class Squeeze

An interaction that represents a squeeze on Apple Pencil.

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

### Apple Pencil interactions in UIKit

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

class Tap

An interaction that represents a double tap on Apple Pencil.

class Squeeze

An interaction that represents a squeeze on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

