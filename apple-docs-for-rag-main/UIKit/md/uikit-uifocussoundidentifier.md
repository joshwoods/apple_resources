

- UIKit
-  UIFocusSoundIdentifier 

Structure

# UIFocusSoundIdentifier

An identifier for a focus-related sound.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UIFocusSoundIdentifier
```

## Mentioned in 

Using custom sounds for focus movement

## Overview

To assign an identifier to a custom sound file, call the register(_:forSoundIdentifier:) method of UIFocusSystem.

## Topics

### Constants

static let `default`: UIFocusSoundIdentifier

The identifier for the default system sound to play during focus updates.

static let none: UIFocusSoundIdentifier

The identifier for disabling sound during a focus update.

### Initializers

init(String)

Creates an identifier for a focus sound.

init(rawValue: String)

Creates an identifier for a focus sound with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the sound to play during updates

Using custom sounds for focus movement

Customize the sounds users hear when focus moves.

func soundIdentifierForFocusUpdate(in: UIFocusUpdateContext) -> UIFocusSoundIdentifier?

Asks the delegate for the identifier of the sound to play when the object gains focus.

