

- UIKit
-  UIInterfaceOrientationMask 

Structure

# UIInterfaceOrientationMask

Constants that specify a view controller’s supported interface orientations.

iOSiPadOSMac CatalystvisionOS

``` source
struct UIInterfaceOrientationMask
```

## Overview

Starting in iOS 8, you should employ the UITraitCollection and UITraitEnvironment APIs, and size class properties as used in those APIs, instead of using UIInterfaceOrientation constants or otherwise writing your app in terms of interface orientation.

In earlier versions of iOS, you returned these constants from the supportedInterfaceOrientations(for:) method or when determining which orientations to support in your app’s view controllers.

## Topics

### Constants

static var portrait: UIInterfaceOrientationMask

The view controller supports a portrait interface orientation.

static var landscapeLeft: UIInterfaceOrientationMask

The view controller supports a landscape-left interface orientation.

static var landscapeRight: UIInterfaceOrientationMask

The view controller supports a landscape-right interface orientation.

static var portraitUpsideDown: UIInterfaceOrientationMask

The view controller supports an upside-down portrait interface orientation.

static var landscape: UIInterfaceOrientationMask

The view controller supports both landscape-left and landscape-right interface orientation.

static var all: UIInterfaceOrientationMask

The view controller supports all interface orientations.

static var allButUpsideDown: UIInterfaceOrientationMask

The view controller supports all but the upside-down portrait interface orientation.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

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

### Managing interface geometry

func application(UIApplication, supportedInterfaceOrientationsFor: UIWindow?) -> UIInterfaceOrientationMask

Asks the delegate for the interface orientations to use for the view controllers in the specified window.

enum UIInterfaceOrientation

Constants that specify the orientation of the app’s user interface.

class let invalidInterfaceOrientationException: NSExceptionName

An exception that’s thrown if a view controller or the app returns an invalid set of supported interface orientations.

