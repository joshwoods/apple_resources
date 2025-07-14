

- UIKit
-  UILayoutGuideAspectFitting 

Protocol

# UILayoutGuideAspectFitting

The interface for a layout guide that supports a particular aspect ratio.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
protocol UILayoutGuideAspectFitting : NSObjectProtocol
```

## Overview

The safeAreaAspectFitLayoutGuide property adopts this protocol to provide a layout guide for placing media content of a particular aspect ratio.

## Topics

### Specifying the aspect ratio

var aspectRatio: CGFloat

The content’s aspect ratio.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working with layout guides

var safeAreaAspectFitLayoutGuide: any UILayoutGuide &amp; UILayoutGuideAspectFitting

A layout guide for placing content of a particular aspect ratio.

