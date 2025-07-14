

- AppKit
- NSView
-  NSView.AutoresizingMask 

Structure

# NSView.AutoresizingMask

Constants that specify the autoresizing behaviors for views.

macOS

``` source
struct AutoresizingMask
```

## Topics

### Getting the Autoresizing mask

static var none: NSView.AutoresizingMask

The view cannot be resized.

static var minXMargin: NSView.AutoresizingMask

The left margin between the view and its superview is flexible.

static var width: NSView.AutoresizingMask

The view’s width is flexible.

static var maxXMargin: NSView.AutoresizingMask

The right margin between the view and its superview is flexible.

static var minYMargin: NSView.AutoresizingMask

The bottom margin between the view and its superview is flexible.

static var height: NSView.AutoresizingMask

The view’s height is flexible.

static var maxYMargin: NSView.AutoresizingMask

The top margin between the view and its superview is flexible.

### Creating an Autoresizing Mask

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

### Resizing Subviews

var autoresizesSubviews: Bool

A Boolean value indicating whether the view applies the autoresizing behavior to its subviews when its frame size changes.

var autoresizingMask: NSView.AutoresizingMask

The options that determine how the view is resized relative to its superview.

func resizeSubviews(withOldSize: NSSize)

Informs the view’s subviews that the view’s bounds rectangle size has changed.

func resize(withOldSuperviewSize: NSSize)

Informs the view that the bounds size of its superview has changed.

