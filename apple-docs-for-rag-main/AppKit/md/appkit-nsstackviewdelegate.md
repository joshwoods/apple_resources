

- AppKit
-  NSStackViewDelegate 

Protocol

# NSStackViewDelegate

A set of methods you use to respond to a stack view detaching and reattaching views.

macOS

``` source
protocol NSStackViewDelegate : NSObjectProtocol
```

## Overview

Adopt this protocol in a custom object and use it to track the addition and removal of views from the stack view’s view hierarchy. For an explanation of detachment and reattachment of a stack view’s views, see NSStackView.

## Topics

### Responding to View Detachment and Reattachment

func stackView(NSStackView, didReattach: [NSView])

Called when the stack view has automatically reattached one or more previously-detached views.

func stackView(NSStackView, willDetach: [NSView])

Called when the stack view is about to automatically detach one or more of its views.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to Stack-Related Changes

var delegate: (any NSStackViewDelegate)?

The delegate object for the stack view.

