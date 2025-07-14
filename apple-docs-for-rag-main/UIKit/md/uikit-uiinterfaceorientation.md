

- UIKit
-  UIInterfaceOrientation 

Enumeration

# UIInterfaceOrientation

Constants that specify the orientation of the app’s user interface.

iOSiPadOSMac CatalystvisionOS

``` source
enum UIInterfaceOrientation
```

## Overview

Starting in iOS 8, you should employ the UITraitCollection and UITraitEnvironment APIs, and size class properties as used in those APIs, instead of using UIInterfaceOrientation constants or otherwise writing your app in terms of interface orientation.

In earlier versions of iOS, you used these constants in the statusBarOrientation property and the setStatusBarOrientation(_:animated:) method.

Important

Notice that UIDeviceOrientation.landscapeRight is assigned to UIInterfaceOrientation.landscapeLeft and UIDeviceOrientation.landscapeLeft is assigned to UIInterfaceOrientation.landscapeRight. The reason for this is that rotating the device requires rotating the content in the opposite direction.

## Topics

### Orientations

case unknown

The orientation of the device is unknown.

case portrait

The device is in portrait mode, with the device upright and the Home button on the bottom.

case portraitUpsideDown

The device is in portrait mode but is upside down, with the device upright and the Home button at the top.

case landscapeLeft

The device is in landscape mode, with the device upright and the Home button on the left.

case landscapeRight

The device is in landscape mode, with the device upright and the Home button on the right.

### Orientation Checks

var isLandscape: Bool

A Boolean value that indicates whether the user interface is currently presented in a landscape orientation.

var isPortrait: Bool

A Boolean value that indicates whether the user interface is currently presented in a portrait orientation.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing interface geometry

func application(UIApplication, supportedInterfaceOrientationsFor: UIWindow?) -> UIInterfaceOrientationMask

Asks the delegate for the interface orientations to use for the view controllers in the specified window.

struct UIInterfaceOrientationMask

Constants that specify a view controller’s supported interface orientations.

class let invalidInterfaceOrientationException: NSExceptionName

An exception that’s thrown if a view controller or the app returns an invalid set of supported interface orientations.

