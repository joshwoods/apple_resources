

- AppKit
- NSStatusItem
-  NSStatusItem.Behavior 

Structure

# NSStatusItem.Behavior

A set of optional status item behaviors.

macOS 10.12+

``` source
struct Behavior
```

## Topics

### Behaviors

static var removalAllowed: NSStatusItem.Behavior

A status item that allows interactive removal.

static var terminationOnRemoval: NSStatusItem.Behavior

A status item that quits the application upon removal.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing the Status Item’s Behavior

var behavior: NSStatusItem.Behavior

The set of allowed behaviors for the status item.

var button: NSStatusBarButton?

The button displayed in the status bar.

var menu: NSMenu?

The pull-down menu displayed when the user clicks the status item.

