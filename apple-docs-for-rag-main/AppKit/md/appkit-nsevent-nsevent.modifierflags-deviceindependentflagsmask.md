

- AppKit
- NSEvent
- NSEvent.ModifierFlags
-  deviceIndependentFlagsMask 

Type Property

# deviceIndependentFlagsMask

Device-independent modifier flags are masked.

macOS

``` source
static var deviceIndependentFlagsMask: NSEvent.ModifierFlags { get }
```

## Discussion

Use this symbol to preserve key event flags and mask all other flags.

## See Also

### Event Modifier Flags

static var capsLock: NSEvent.ModifierFlags

The Caps Lock key has been pressed.

static var shift: NSEvent.ModifierFlags

The Shift key has been pressed.

static var control: NSEvent.ModifierFlags

The Control key has been pressed.

static var option: NSEvent.ModifierFlags

The Option or Alt key has been pressed.

static var command: NSEvent.ModifierFlags

The Command key has been pressed.

static var numericPad: NSEvent.ModifierFlags

A key in the numeric keypad or an arrow key has been pressed.

static var help: NSEvent.ModifierFlags

The Help key has been pressed.

static var function: NSEvent.ModifierFlags

A function key has been pressed.

