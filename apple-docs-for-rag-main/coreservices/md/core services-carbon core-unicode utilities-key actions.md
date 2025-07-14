

- Core Services
- Carbon Core
- Unicode Utilities
-  Key Actions 

# Key Actions

Indicate the current key action.

## Overview

You can supply the following constants for the `keyAction` parameter of the function UCKeyTranslate(_:_:_:_:_:_:_:_:_:_:) to indicate the current key action.

## Topics

### Constants

var kUCKeyActionDown: Int

The user is pressing the key.

var kUCKeyActionUp: Int

The user is releasing the key.

var kUCKeyActionAutoKey: Int

The user has the key in an “auto-key” pressed state that is, the user is holding down the key for an extended period of time and is thereby generating multiple key strokes from the single key.

var kUCKeyActionDisplay: Int

The user is requesting information for key display, as in the Key Caps application.

