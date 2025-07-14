

- AppKit
- NSEvent
-  NSEvent.SpecialKey 

Structure

# NSEvent.SpecialKey

Constants for reserved function keys on the keyboard.

macOS 10.9+

``` source
struct SpecialKey
```

## Overview

These constants correspond to unicode characters in the range (0xF700–0xF8FF) and are values you can use with the characters and charactersIgnoringModifiers properties of the event. You can also use them in some parameters in the keyEvent(with:location:modifierFlags:timestamp:windowNumber:context:characters:charactersIgnoringModifiers:isARepeat:keyCode:) method of the event.

Note that the system handles some function keys at a lower level and your app never sees them. Examples include the Volume Up key, Volume Down key, Volume Mute key, Eject key, and Function key found on many Macs.

## Topics

### Getting Common Control Keys

static let backspace: NSEvent.SpecialKey

The backspace key.

static let carriageReturn: NSEvent.SpecialKey

The carriage return key.

static let newline: NSEvent.SpecialKey

The newline key.

static let enter: NSEvent.SpecialKey

The enter key.

static let delete: NSEvent.SpecialKey

The delete key.

static let deleteForward: NSEvent.SpecialKey

The delete forward key.

static let backTab: NSEvent.SpecialKey

The back tab key.

static let tab: NSEvent.SpecialKey

The tab key.

### Getting the Navigation-Related Keys

static let upArrow: NSEvent.SpecialKey

The up arrow key.

static let downArrow: NSEvent.SpecialKey

The down arrow key.

static let leftArrow: NSEvent.SpecialKey

The left arrow key.

static let rightArrow: NSEvent.SpecialKey

The right arrow key.

static let pageUp: NSEvent.SpecialKey

The page up key.

static let pageDown: NSEvent.SpecialKey

The page down key.

static let home: NSEvent.SpecialKey

The home key.

static let end: NSEvent.SpecialKey

The end key.

static let prev: NSEvent.SpecialKey

The previous key.

static let next: NSEvent.SpecialKey

The next key.

### Getting Special Behavior Keys

static let begin: NSEvent.SpecialKey

The begin key.

static let `break`: NSEvent.SpecialKey

The break key.

static let clearDisplay: NSEvent.SpecialKey

The clear display key.

static let clearLine: NSEvent.SpecialKey

The clear line key.

static let deleteCharacter: NSEvent.SpecialKey

The delete character key.

static let deleteLine: NSEvent.SpecialKey

The delete line key.

static let execute: NSEvent.SpecialKey

The execute key.

static let find: NSEvent.SpecialKey

The find key.

static let formFeed: NSEvent.SpecialKey

The form feed key.

static let help: NSEvent.SpecialKey

The help key.

static let insert: NSEvent.SpecialKey

The insert key.

static let insertCharacter: NSEvent.SpecialKey

The insert character key.

static let insertLine: NSEvent.SpecialKey

The insert line key.

static let lineSeparator: NSEvent.SpecialKey

The line separator key.

static let menu: NSEvent.SpecialKey

The menu key.

static let modeSwitch: NSEvent.SpecialKey

The mode switch key.

static let paragraphSeparator: NSEvent.SpecialKey

The paragraph separator key.

static let pause: NSEvent.SpecialKey

The pause key.

static let print: NSEvent.SpecialKey

The print key.

static let printScreen: NSEvent.SpecialKey

The print screen key.

static let redo: NSEvent.SpecialKey

The redo key.

static let reset: NSEvent.SpecialKey

The reset key.

static let scrollLock: NSEvent.SpecialKey

The scroll lock key.

static let select: NSEvent.SpecialKey

The select key.

static let stop: NSEvent.SpecialKey

The stop key.

static let sysReq: NSEvent.SpecialKey

The system request key.

static let system: NSEvent.SpecialKey

The system key.

static let undo: NSEvent.SpecialKey

The undo key.

static let user: NSEvent.SpecialKey

The user key.

### Getting the Function Keys

static let f1: NSEvent.SpecialKey

The F1 key.

static let f2: NSEvent.SpecialKey

The F2 key.

static let f3: NSEvent.SpecialKey

The F3 key.

static let f4: NSEvent.SpecialKey

The F4 key.

static let f5: NSEvent.SpecialKey

The F5 key.

static let f6: NSEvent.SpecialKey

The F6 key.

static let f7: NSEvent.SpecialKey

The F7 key.

static let f8: NSEvent.SpecialKey

The F8 key.

static let f9: NSEvent.SpecialKey

The F9 key.

static let f10: NSEvent.SpecialKey

The F10 key.

static let f11: NSEvent.SpecialKey

The F11 key.

static let f12: NSEvent.SpecialKey

The F12 key.

static let f13: NSEvent.SpecialKey

The F13 key.

static let f14: NSEvent.SpecialKey

The F14 key.

static let f15: NSEvent.SpecialKey

The F15 key.

static let f16: NSEvent.SpecialKey

The F16 key.

static let f17: NSEvent.SpecialKey

The F17 key.

static let f18: NSEvent.SpecialKey

The F18 key.

static let f19: NSEvent.SpecialKey

The F19 key.

static let f20: NSEvent.SpecialKey

The F20 key.

static let f21: NSEvent.SpecialKey

The F21 key.

static let f22: NSEvent.SpecialKey

The F22 key.

static let f23: NSEvent.SpecialKey

The F23 key.

static let f24: NSEvent.SpecialKey

The F24 key.

static let f25: NSEvent.SpecialKey

The F25 key.

static let f26: NSEvent.SpecialKey

The F26 key.

static let f27: NSEvent.SpecialKey

The F27 key.

static let f28: NSEvent.SpecialKey

The F28 key.

static let f29: NSEvent.SpecialKey

The F29 key.

static let f30: NSEvent.SpecialKey

The F30 key.

static let f31: NSEvent.SpecialKey

The F31 key.

static let f32: NSEvent.SpecialKey

The F32 key.

static let f33: NSEvent.SpecialKey

The F33 key.

static let f34: NSEvent.SpecialKey

The F34 key.

static let f35: NSEvent.SpecialKey

The F35 key.

### Getting the Key’s Value

var unicodeScalar: Unicode.Scalar

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

## See Also

### Getting key event information

var characters: String?

The characters associated with a key-up or key-down event.

var charactersIgnoringModifiers: String?

The characters generated by a key event as if no modifier key (except for Shift) applies.

var keyCode: UInt16

The virtual code for the key associated with the event.

func characters(byApplyingModifiers: NSEvent.ModifierFlags) -> String?

Returns the new characters that result if you apply the specified modifier keys to the event.

class var keyRepeatDelay: TimeInterval

The number of seconds someone must hold down a key before the first key repeat event occurs.

class var keyRepeatInterval: TimeInterval

The number of seconds someone must hold down a key to generate key-repeat events after the initial delay.

var specialKey: NSEvent.SpecialKey?

The code associated with a function key or other special key.

Function-Key Unicode Values

Constants for reserved keyboard function keys that correspond to unicode characters.

var isARepeat: Bool

A Boolean value that indicates whether the key event is a repeat.

