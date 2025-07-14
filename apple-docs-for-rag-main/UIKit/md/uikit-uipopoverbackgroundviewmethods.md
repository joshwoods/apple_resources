

- UIKit
-  UIPopoverBackgroundViewMethods 

Protocol

# UIPopoverBackgroundViewMethods

A set of methods that popover background view subclasses must implement.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
protocol UIPopoverBackgroundViewMethods
```

## Overview

The methods in this protocol are called only once when the popover is presented. All methods of this protocol are required.

## Topics

### Returning the content view insets

static func contentViewInsets() -> UIEdgeInsets

The insets for the content portion of the popover.

**Required**

### Accessing the arrow metrics

static func arrowBase() -> CGFloat

The width of the arrow triangle at its base.

**Required**

static func arrowHeight() -> CGFloat

The height of the arrow (measured in points) from its base to its tip.

**Required**

## Relationships

### Conforming Types

- UIPopoverBackgroundView

## See Also

### Popovers

Displaying transient content in a popover

Show a temporary interface on top of your app’s content on iPad.

class UIPopoverPresentationController

An object that manages the display of content in a popover.

class UIPopoverBackgroundView

The background appearance for a popover.

