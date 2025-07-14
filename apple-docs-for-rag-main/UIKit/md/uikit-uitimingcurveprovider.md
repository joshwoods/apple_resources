

- UIKit
-  UITimingCurveProvider 

Protocol

# UITimingCurveProvider

An interface for providing the timing information needed to perform animations.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITimingCurveProvider : NSCoding, NSCopying
```

## Overview

An object that adopts the UITimingCurveProvider protocol provides the timing information needed to perform animations with a UIViewPropertyAnimator object. A timing curve defines the velocity at which animated properties change to their new values over the duration of the animation. A custom timing curve provider can specify timing using the built-in UIKit curves, a cubic Bézier curve, a spring-based timing function, or a combination of timing information.

When implementing this protocol in a custom object, you must provide implementations for all of the properties. Use the timingCurveType property to specify which timing information your object provides. Configure the other properties with the actual timing curve values.

## Topics

### Getting the timing information

var timingCurveType: UITimingCurveType

The type of timing information to use.

**Required**

var cubicTimingParameters: UICubicTimingParameters?

The cubic timing parameters to use.

**Required**

var springTimingParameters: UISpringTimingParameters?

The spring-based timing parameters to use.

**Required**

### Constants

enum UITimingCurveType

Constants indicating the type of timing information to use.

## Relationships

### Inherits From

- NSCoding
- NSCopying

### Conforming Types

- UICubicTimingParameters
- UISpringTimingParameters

## See Also

### Timing curves

class UISpringTimingParameters

The timing information for animations that mimics the behavior of a spring.

class UICubicTimingParameters

The timing information for animations in the form of a cubic Bézier curve.

