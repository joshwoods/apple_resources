

- AppKit
-  NSMatrixDelegate 

Protocol

# NSMatrixDelegate

The `NSMatrixDelegate` protocol defines the optional methods implemented by delegates of `NSMatrix` objects.

macOS

``` source
protocol NSMatrixDelegate : NSControlTextEditingDelegate
```

## Overview

This protocol simply adopts the `NSControlTextEditingDelegate` protocol, adding no additional methods. See NSControlTextEditingDelegate for more information.

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol

## See Also

### Related Documentation

Matrix Programming Guide

### Managing the Delegate

var delegate: (any NSMatrixDelegate)?

The delegate for messages from the field editor.

