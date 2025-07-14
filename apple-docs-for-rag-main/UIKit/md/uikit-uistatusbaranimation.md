

- UIKit
-  UIStatusBarAnimation 

Enumeration

# UIStatusBarAnimation

Constants that specify the animation of the status bar as it’s hidden or made visible.

iOSiPadOSMac CatalystvisionOS

``` source
enum UIStatusBarAnimation
```

## Overview

Constants of the UIStatusBarAnimation type are arguments of the setStatusBarHidden(_:with:) method.

## Topics

### Constants

case none

No animation is applied to the status bar as it is shown or hidden.

case fade

The status bar fades in and out as it is shown or hidden, respectively.

case slide

The status bar slides in or out as it is shown or hidden, respectively.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

