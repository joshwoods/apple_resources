

- UIKit
-  UISceneSizeRestrictions 

Class

# UISceneSizeRestrictions

An object that specifies the minimum and maximum sizes for resizable windows.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UISceneSizeRestrictions
```

## Overview

Don’t create a UISceneSizeRestrictions object yourself. Instead, fetch an existing one from the sizeRestrictions property of your window scene, and modify its properties to set the minimum and maximum window sizes. The system provides this object only when it supports variable-sized windows.

## Topics

### Setting the size restrictions

var minimumSize: CGSize

The minimum width and height supported by your app’s windows.

var maximumSize: CGSize

The maximum width and height supported by your app’s windows.

var allowsFullScreen: Bool

A Boolean value that indicates whether the scene can appear full screen.

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

### Getting the interface attributes

var traitCollection: UITraitCollection

The traits that describe the current environment of the scene.

var coordinateSpace: any UICoordinateSpace

The coordinate space occupied by the scene.

var interfaceOrientation: UIInterfaceOrientation

The orientation to use when displaying content in your windows.

var sizeRestrictions: UISceneSizeRestrictions?

The minimum and maximum size of the app’s windows.

