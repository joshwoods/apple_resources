

- UIKit
-  UILayoutSupport 

Protocol

# UILayoutSupport

A set of methods that provide layout support and access to layout anchors.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UILayoutSupport : NSObjectProtocol
```

## Overview

This protocol is implemented by the UIViewController properties topLayoutGuide and bottomLayoutGuide to support using Auto Layout with a view controller’s view. You can use layout guides as layout items in the NSLayoutConstraint factory methods.

## Topics

### Creating constraints using layout anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the guide’s bottom edge.

**Required**

var heightAnchor: NSLayoutDimension

A layout anchor representing the guide’s height.

**Required**

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the guide’s top edge.

**Required**

### Performing layout calculations

var length: CGFloat

Provides the length, in points, of the portion of a view controller’s view that is overlaid by translucent or transparent UIKit bars.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Constraints

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

Positioning content relative to the safe area

Position views so that they aren’t obstructed by other content.

class NSLayoutConstraint

The relationship between two user interface objects that must be satisfied by the constraint-based layout system.

