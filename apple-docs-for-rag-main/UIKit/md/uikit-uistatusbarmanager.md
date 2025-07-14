

- UIKit
-  UIStatusBarManager 

Class

# UIStatusBarManager

An object that describes the configuration of the status bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIStatusBarManager
```

## Overview

Use a UIStatusBarManager object to get the current configuration of the status bar for its associated scene. You don’t create UIStatusBarManager objects directly. Instead, you retrieve an existing object from the statusBarManager property of a UIWindowScene object.

You don’t use this object to modify the configuration of the status bar. Instead, you set the status bar configuration individually for each of your UIViewController objects. For example, to modify the default visibility of the status bar, override the prefersStatusBarHidden property of your view controller.

## Topics

### Getting the status bar configuration

var isStatusBarHidden: Bool

A Boolean value that indicates whether the status bar is currently hidden.

var statusBarStyle: UIStatusBarStyle

The current appearance of the status bar.

### Getting the frame rectangle

var statusBarFrame: CGRect

The frame rectangle of the status bar.

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

## See Also

### Device environment

class UIDevice

A representation of the current device.

